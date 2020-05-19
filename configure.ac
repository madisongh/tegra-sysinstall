dnl
dnl configure.ac - autoconf script for tegra-sysinstall
dnl
dnl Copyright (c) 2019, 2020 Matthew Madison
dnl
AC_INIT([tegra-sysinstall], [1.2.0])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MAJOR], [1], [Major version])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MINOR], [2], [Minor version])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MAINT], [0], [Maintenance level])
AM_INIT_AUTOMAKE([subdir-objects foreign])
AM_SILENT_RULES([yes])
AC_COPYRIGHT([
Copyright (c) 2019, 2020 Matthew Madison
])
AC_CONFIG_MACRO_DIR([m4])

AC_PREREQ([2.69])
LT_PREREQ([2.4])
LT_INIT([])

AC_CANONICAL_HOST
AC_PROG_INSTALL

AC_CONFIG_FILES(Makefile src/tegra-sysinstall src/tegra-sysinstall-menu lib/tools-common lib/menu-common)
AC_OUTPUT
