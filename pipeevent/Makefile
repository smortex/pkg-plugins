.include <bsd.own.mk>

PREFIX?=	/usr/local
LIBDIR=		${PREFIX}/lib/pkg/
SHLIB_DIR?=	${LIBDIR}/
SHLIB_NAME?=	${PLUGIN_NAME}.so

PLUGIN_NAME=	pipeevent
SRCS=		pipeevent.c

PKGFLAGS!=	pkgconf --cflags pkg
CFLAGS+=	${PKGFLAGS}

beforeinstall:
	${INSTALL} -d ${LIBDIR}

.include <bsd.lib.mk>
