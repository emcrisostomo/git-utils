#                                               -*- Autoconf -*-
# Copyright (C) 2016-2018 Enrico M. Crisostomo
#
# This program is free software; you can redistribute it and/or modify it under
# the terms of the GNU General Public License as published by the Free Software
# Foundation; either version 3, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
# FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
# details.
#
# You should have received a copy of the GNU General Public License along with
# this program.  If not, see <http://www.gnu.org/licenses/>.
#
# Process this file with autoconf to produce a configure script.
#
dnl Copyright (C) 2016-2018 Enrico M. Crisostomo
AC_PREREQ([2.69])
AC_INIT([git-utils], [1.3.2], [enrico.m.crisostomo@gmail.com])
AC_COPYRIGHT([2016-2018 (C) Enrico M. Crisostomo])
AC_REVISION([$Revision: 1.0.0$])
AC_CONFIG_SRCDIR([scripts/git-outgoing.in])
AC_CONFIG_SRCDIR([scripts/git-pull-all.in])
AC_CONFIG_AUX_DIR([config])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([scripts/git-outgoing], [chmod +x scripts/git-outgoing])
AC_CONFIG_FILES([scripts/git-pull-all], [chmod +x scripts/git-pull-all])
AC_CONFIG_MACRO_DIRS([m4])
AC_CONFIG_MACRO_DIR([m4])

# Initialize Automake
AM_INIT_AUTOMAKE([-Wall -Werror gnu subdir-objects])
AM_SILENT_RULES([yes])

# Checks for programs.
AC_PATH_PROG([ZSH_CMD], [zsh], [no])
AC_PATH_PROG([GIT_CMD], [git], [no])

AS_VAR_IF([ZSH_CMD], [no], [AC_MSG_ERROR([zsh is required.])], [])
AS_VAR_IF([GIT_CMD], [no], [AC_MSG_ERROR([git is required.])], [])

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_OUTPUT
