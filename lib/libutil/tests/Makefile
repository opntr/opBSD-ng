# $FreeBSD$

TAP_TESTS_C+=	flopen_test
TAP_TESTS_C+=	grp_test
TAP_TESTS_C+=	humanize_number_test
TAP_TESTS_C+=	pidfile_test
TAP_TESTS_C+=	trimdomain_test
TAP_TESTS_C+=	trimdomain-nodomain_test

DPADD+=		${LIBUTIL}
LDADD+=		-lutil
WARNS?=		2

.include <bsd.test.mk>
