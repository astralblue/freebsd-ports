# $FreeBSD$

PORTNAME=	qwalk
DISTVERSIONPREFIX=	v
DISTVERSION=	1.0.1-300
DISTVERSIONSUFFIX=	-g1b7e381
CATEGORIES=	science

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Quantum Monte Carlo package for quantum chemistry computations

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/../COPYING

USES=		fortran gmake perl5
USE_GITHUB=	yes
GH_ACCOUNT=	QWalk
GH_PROJECT=	mainline
USE_GNOME=	libxml2

WRKSRC_SUBDIR=	src
MAKE_ARGS=	INSTALLPATH=${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
