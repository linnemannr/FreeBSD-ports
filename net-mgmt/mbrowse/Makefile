# Created by: Mark Pulford <mark@kyne.com.au>
# $FreeBSD$

PORTNAME=	mbrowse
PORTVERSION=	0.4.3
CATEGORIES=	net-mgmt
MASTER_SITES=	SF/${PORTNAME}/${PORTVERSION}

MAINTAINER=	eg@fbsd.lt
COMMENT=	SNMP MIB Browser for X

LICENSE=	GPLv2

LIB_DEPENDS=	libnetsnmp.so:net-mgmt/net-snmp

GNU_CONFIGURE=	yes
PLIST_FILES=	bin/mbrowse
USES=		gnome pkgconfig
USE_GNOME=	gtk20
CONFIGURE_ARGS=	--with-snmp-prefix=${PREFIX} --with-snmp-type=net
CPPFLAGS+=	`net-snmp-config --cflags`
LDFLAGS+=	`net-snmp-config --libs`

.include <bsd.port.mk>
