# $NetBSD: Makefile,v 1.4 2012/10/23 18:16:48 asau Exp $

PKGNAME=	${DISTNAME:S/_/-/}
DISTNAME=	pam_radius-1.3.16
CATEGORIES=	security
MASTER_SITES=	ftp://ftp.freeradius.org/pub/radius/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://www.freeradius.org/pam_radius_auth/
COMMENT=	PAM module for authentication against a RADIUS server

NO_CONFIGURE=	YES
EXTRACT_SUFX=	.tar

INSTALLATION_DIRS=	lib/security share/doc/pam-radius share/examples/pam-radius

do-install:
	${INSTALL_DATA} ${WRKSRC}/INSTALL ${DESTDIR}${PREFIX}/share/doc/pam-radius
	${INSTALL_DATA} ${WRKSRC}/README ${DESTDIR}${PREFIX}/share/doc/pam-radius
	${INSTALL_DATA} ${WRKSRC}/USAGE ${DESTDIR}${PREFIX}/share/doc/pam-radius
	${INSTALL_DATA} ${WRKSRC}/pam_radius_auth.conf \
		${DESTDIR}${PREFIX}/share/examples/pam-radius
	${INSTALL_LIB} ${WRKSRC}/pam_radius_auth.so ${DESTDIR}${PREFIX}/lib/security

.include "../../mk/pam.buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
