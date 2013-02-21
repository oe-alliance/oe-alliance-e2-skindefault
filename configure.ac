AC_INIT([enigma2-skindefault],[1.0])
AM_INIT_AUTOMAKE([dist-bzip2 foreign no-define tar-pax])
AC_CONFIG_HEADERS([enigma2-plugins-config.h])

# Silent rules are available since 1.11, but older versions
# are still in use. So don't use them unconditionally.
m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

AC_USE_SYSTEM_EXTENSIONS
AC_SYS_LARGEFILE

AC_PROG_CC
AC_PROG_CXX
m4_ifdef([LT_INIT], [LT_INIT], [AC_PROG_LIBTOOL])
AC_CONFIG_MACRO_DIR([m4])

AC_CHECK_HEADERS([dbox/fp.h dbox/lcd-ks0713.h])

AM_PATH_PYTHON
AX_PYTHON_DEVEL
AX_PTHREAD

TUXBOX_APPS_DVB

AC_CONFIG_FILES([
Makefile
fonts/Makefile
skin_default/Makefile
skin_default/buttons/Makefile
skin_default/countries/Makefile
skin_default/epg/Makefile
skin_default/extensions/Makefile
skin_default/icons/Makefile
skin_default/infobar/Makefile
skin_default/piconbg/Makefile
skin_default/screens/Makefile
])
AC_OUTPUT
