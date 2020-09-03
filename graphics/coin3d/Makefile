# $OpenBSD$

COMMENT =		3D graphics library

V =			4.0.0
DISTNAME =		coin
PKGNAME =		libcoin-${V}

CATEGORIES =		graphics

HOMEPAGE =		https://github.com/coin3d/coin

MAINTAINER =		Charlie Burnett <burne251@umn.edu>

# BSD3
PERMIT_PACKAGE =	Yes

DISTFILES =		coin-${V}-src${EXTRACT_SUFX}

MASTER_SITES =		https://github.com/coin3d/coin/releases/download/Coin-${V}/

LIB_DEPENDS =		devel/boost

CONFIGURE_ARGS+=	--enable-3ds-import --enable-threadsafe

CONFIGURE_ENV= 		CPPFLAGS="${CPPFLAGS} -I/usr/local/include"

CPPFLAGS+=		"-I/usr/local/include"

LIBCoin_VERSION=	4

SEPARATE_BUILD =	Yes

CONFIGURE_STYLE =	gnu

pre-configure:
	chmod +x ${WRKSRC}/configure

.include <bsd.port.mk>
