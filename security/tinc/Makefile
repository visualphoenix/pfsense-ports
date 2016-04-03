# Created by: ijliao
# $FreeBSD$

PORTNAME=	tinc
PORTVERSION=	1.2
PORTREVISION=	1
CATEGORIES=	security

USE_GITHUB=	yes
GH_ACCOUNT=	gsliepen
GH_PROJECT=	tinc
GH_TAGNAME=	e44c337

MAINTAINER=	dinoex@FreeBSD.org
COMMENT=	Virtual Private Network (VPN) daemon

LICENSE=	GPLv3

LIB_DEPENDS=	liblzo2.so:${PORTSDIR}/archivers/lzo2


USES=		autoreconf
CPE_VENDOR=	tinc-vpn
USE_OPENSSL=	yes
GNU_CONFIGURE=	yes
CPPFLAGS+=	-I${LOCALBASE}/include
LDFLAGS+=	-L${LOCALBASE}/lib
CONFIGURE_ARGS=	--localstatedir=/var
USE_RC_SUBR=	tincd
INFO=		tinc
PLIST_FILES=	sbin/tincd \
		sbin/tinc \
		sbin/sptps_keypair \
		sbin/sptps_speed \
		sbin/sptps_test \
		man/man5/tinc.conf.5.gz man/man8/tincd.8.gz

.include <bsd.port.mk>
