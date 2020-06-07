# $OpenBSD$


COMMENT = 		a CAM-related software for pocketing operations
CATEGORIES = 		devel
HOMEPAGE = 		https://github.com/Heeks/libarea
VERSION = 		0.0.20191031
DISTNAME = 		libarea-${VERSION}
PKGNAME = 		${DISTNAME}
MAINTAINER = 		Charlie Burnett <burne251@umn.edu>
PERMIT_PACKAGE=		Yes
GH_ACCOUNT =		Heeks
GH_PROJECT = 		libarea
GH_COMMIT = 		2752cd989f53e9e2f52663e731ebfdf3bff2ebe8

# BSD 3-Clause License

SHARED_LIBS +=		libarea.so			0.0

LIB_DEPENDS += 		devel/boost

PY-VER = 		"3.7"

MAKE_ENV +=		CPLUS_INCLUDE_PATH="${CPLUS_INCLUDE_PATH}/usr/local/include/python${PY-VER}m/"

MODULES += 		devel/cmake

WANTLIB += 		${COMPILER_LIBCXX} m boost_python-mt

.include <bsd.port.mk>
