# $NetBSD: Makefile,v 1.12 2013/06/04 22:16:10 tron Exp $
#

DISTNAME=	qonk-0.3.1
PKGREVISION=	8
CATEGORIES=	games
MASTER_SITES=	${MASTER_SITE_SOURCEFORGE:=qonk/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://qonk.sourceforge.net/
COMMENT=	Small space build-and-conquer strategy game
LICENSE=	gnu-gpl-v2

GNU_CONFIGURE=	yes
USE_LANGUAGES=	c c++

.include "../../devel/SDL/buildlink3.mk"
.include "../../devel/SDL_ttf/buildlink3.mk"
.include "../../devel/SDL_gfx/buildlink3.mk"
.include "../../graphics/SDL_image/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
