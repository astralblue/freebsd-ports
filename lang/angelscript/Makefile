# Created by: Veniamin Gvozdikov <vg@FreeBSD.org>
# $FreeBSD$

PORTNAME=	angelscript
PORTVERSION=	2.32.0
CATEGORIES=	lang
MASTER_SITES=	http://www.angelcode.com/angelscript/sdk/files/
DISTNAME=	${PORTNAME}_${PORTVERSION}

MAINTAINER=	ndowens@yahoo.com
COMMENT=	AngelCode Scripting Library

LICENSE=	ZLIB

BROKEN_aarch64=	Does not build: invokes x86 asm
BROKEN_powerpc64=	Does not build: invokes x86 asm
BROKEN_sparc64=	Does not build: invokes x86 asm

USES=		alias gmake zip
USE_LDCONFIG=	yes

MAKE_ARGS=	CP_SYMLINK="${INSTALL_LIB}"

.include <bsd.port.options.mk>
.if ${ARCH} == "i386"
USE_GCC=	yes
.endif

WRKSRC=		${WRKDIR}/sdk/angelscript/projects/gnuc/

PLIST_FILES=	include/angelscript.h \
		lib/libangelscript.a \
		lib/libangelscript.so \
		lib/libangelscript.so.${PORTVERSION}

.include <bsd.port.mk>
