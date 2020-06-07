# $OpenBSD$

COMMENT =		store and exchange meshed data or computation results

V =			4.0.0
DISTNAME =		med-${V}
PKGNAME =		libmedc-${V}

SHARED_LIBS +=		med		0.0 # 11.0
SHARED_LIBS +=  	medC		0.0 # 11.0
SHARED_LIBS +=  	medimport	0.0 # 3.0

CATEGORIES =		math graphics

HOMEPAGE =		https://www.salome-platform.org/

MAINTAINER =		Paco Esteban <paco@openbsd.org>

# LGPLv3
PERMIT_PACKAGE =	Yes

MASTER_SITES =		http://files.salome-platform.org/Salome/other/

WANTLIB +=		${COMPILER_LIBCXX} c hdf5 m z

MODULES =		fortran

BUILD_DEPENDS =		textproc/gsed

LIB_DEPENDS =		math/hdf5

USE_GMAKE =		Yes
CONFIGURE_STYLE =	gnu
CONFIGURE_ARGS =	--disable-python \
			--with-hdf5=${LOCALBASE} \
			--with-hdf5-bin=${LOCALBASE}/bin

.include <bsd.port.mk>
