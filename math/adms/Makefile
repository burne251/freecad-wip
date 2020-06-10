#; $OpenBSD: Makefile,v 1.6 2020/03/14 06:39:03 rsadowski Exp $

COMMENT =	library for doing god knows what
CATEGORIES = 	devel

GH_ACCOUNT = 	qucs
GH_PROJECT = 	ADMS
GH_TAGNAME = 	release-2.3.6

CATEGORIES =	devel

# GPLv2
PERMIT_PACKAGE =	Yes


MODULES += 		devel/cmake

RUN_DEPENDS += 		textproc/p5-XML-LibXML \
			textproc/p5-XML-NamespaceSupport \
			textproc/p5-XML-SAX \
			textproc/p5-XML-SAX-Base \
			converters/libiconv \
			textproc/libxml \
			archivers/xz


CONFIGURE_ARGS += 	-DUSE_MAINTAINER_MODE=ON \
			-DCMAKE_BUILD_TYPE=RELEASE \
			-DCMAKE_INSTALL_PREFIX=/usr/local/


COMPILER =	base-clang ports-gcc base-gcc


CFLAGS += 		-I/usr/local/include
LDFLAGS += 		-L/usr/local/lib

WANTLIB += 		c m

.include <bsd.port.mk>
