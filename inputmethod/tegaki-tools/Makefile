# $NetBSD: Makefile,v 1.4 2014/01/25 10:30:12 wiz Exp $

DISTNAME=	tegaki-tools-0.3.1
PKGREVISION=	1
CATEGORIES=	inputmethod
MASTER_SITES=	http://www.tegaki.org/releases/${PKGVERSION_NOREV}/

MAINTAINER=	obache@NetBSD.org
HOMEPAGE=	http://www.tegaki.org/
COMMENT=	Set of command-line tools for Tegaki
LICENSE=	gnu-gpl-v2

DEPENDS+=	tegaki-python>=0.3:../../inputmethod/tegaki-python
DEPENDS+=	tegaki-pygtk>=0.3:../../inputmethod/tegaki-pygtk

USE_LANGUAGES=	c c++

PYTHON_VERSIONS_INCOMPATIBLE=	33 # not yet ported as of 0.3.1
EGG_NAME=	${DISTNAME:S/-/_/}

.include "../../lang/python/application.mk"
.include "../../lang/python/distutils.mk"
.include "../../mk/bsd.pkg.mk"
