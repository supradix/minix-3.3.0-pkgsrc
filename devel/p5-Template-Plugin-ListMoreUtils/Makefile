# $NetBSD: Makefile,v 1.7 2013/05/31 12:40:45 wiz Exp $
#

DISTNAME=	Template-Plugin-ListMoreUtils-0.02
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	4
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Template/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/Template-Plugin-ListMoreUtils/
COMMENT=	TT2 plugin to use List::MoreUtils
LICENSE=	${PERL5_LICENSE}

USE_LANGUAGES=		# empty

DEPENDS+=	p5-List-MoreUtils>=0.22:../../devel/p5-List-MoreUtils
DEPENDS+=	p5-Template-Plugin-VMethods>=0.02:../../devel/p5-Template-Plugin-VMethods
DEPENDS+=	p5-Template-Toolkit>=2.22:../../www/p5-Template-Toolkit

PERL5_PACKLIST=		auto/Template/Plugin/ListMoreUtils/.packlist
PERL5_MODULE_TYPE=	Module::Build

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
