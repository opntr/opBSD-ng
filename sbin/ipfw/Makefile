# $FreeBSD$

.include <bsd.own.mk>

PROG=	ipfw
SRCS=	ipfw2.c dummynet.c ipv6.c main.c nat.c
WARNS?=	2

.if ${MK_PF} != "no"
SRCS+=	altq.c
CFLAGS+=-DPF
.endif

DPADD=	${LIBJAIL} ${LIBUTIL}
LDADD=	-ljail -lutil
MAN=	ipfw.8

.include <bsd.prog.mk>
