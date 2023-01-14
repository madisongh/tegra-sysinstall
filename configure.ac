dnl
dnl configure.ac - autoconf script for tegra-sysinstall
dnl
dnl Copyright (c) 2019-2023, Matthew Madison
dnl
AC_INIT([tegra-sysinstall], [1.8.0])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MAJOR], [1], [Major version])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MINOR], [8], [Minor version])
AC_DEFINE([TEGRA_SYSINSTALL_VERSION_MAINT], [0], [Maintenance level])
AM_INIT_AUTOMAKE([subdir-objects foreign])
AM_SILENT_RULES([yes])
AC_COPYRIGHT([
Copyright (c) 2019-2023, Matthew Madison
])
AC_CONFIG_MACRO_DIR([m4])

AC_PREREQ([2.69])
LT_PREREQ([2.4])
LT_INIT([])

AC_CANONICAL_HOST
AC_PROG_INSTALL

AC_ARG_WITH([partition-alignment],
	AS_HELP_STRING([--with-partition-alignment=N], [alignment setting for partitions in sectors]),
	[], [with_partition_alignment=1])
AC_SUBST([PARTALIGN], [$with_partition_alignment])

AC_ARG_WITH([key-retrieval-command],
	AS_HELP_STRING([--with-key-retrieval-command=CMD],
	[command to retrieve key which is used as LUKS passphrase @<:@default="keystoretool -p"@:>@]),
	[], [with_key_retrieval_command="keystoretool -p"])
AC_SUBST([KEY_RETRIEVAL_CMD], [$with_key_retrieval_command])

AC_CONFIG_FILES(Makefile src/tegra-sysinstall src/tegra-sysinstall-menu lib/tools-common lib/menu-common)
AC_OUTPUT
