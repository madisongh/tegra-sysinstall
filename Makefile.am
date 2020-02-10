# tegra-sysinstall makefile
#
# Copyright (c) 2019, 2020 Matthew Madison
#

AUTOMAKE_OPTIONS = subdir-objects foreign
ACLOCAL_AMFLAGS = -I m4
SUBDIRS =
DIST_SUBDIRS =

prefix = /usr
exec_prefix = /usr
datadir = $(prefix)/share
sbindir = $(exec_prefix)/sbin

toolsdir = $(datadir)/tegra-sysinstall

EXTRA_DIST = src/tegra-sysinstall.in src/tegra-sysinstall-menu.in \
		lib/tools-common.in lib/menu-common.in

tools_DATA = lib/tools-common lib/menu-common
dist_sbin_SCRIPTS = src/tegra-sysinstall src/tegra-sysinstall-menu
