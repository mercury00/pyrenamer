###################################
### Initialization
###################################
AC_INIT([pyrenamer], [0.7.0])
AC_CONFIG_SRCDIR(src/pyrenamer)
AM_INIT_AUTOMAKE([1.7])
AM_MAINTAINER_MODE


###################################
### Python modules
###################################
AM_PATH_PYTHON
PKG_CHECK_MODULES(PYGOBJECT, PyGObject)
AC_SUBST(PYGOBJECT_CFLAGS)
AC_SUBST(PYGOBJECT_LIBS)


###################################
### Internationalization
###################################
GETTEXT_PACKAGE=pyrenamer
AC_SUBST([GETTEXT_PACKAGE])
AC_DEFINE_UNQUOTED([GETTEXT_PACKAGE], "$GETTEXT_PACKAGE", [Gettext package])
AM_GLIB_GNU_GETTEXT
IT_PROG_INTLTOOL([0.35.0])


###################################
### Config and output
###################################
AC_CONFIG_FILES([
	Makefile
	data/Makefile
	data/pyrenamer.desktop.in.in
	doc/Makefile
	images/Makefile
	po/Makefile.in
	src/Makefile
])
AC_OUTPUT
