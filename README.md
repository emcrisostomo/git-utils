[![License](https://img.shields.io/badge/license-GPL--3.0-blue.svg?style=flat)](https://github.com/emcrisostomo/git-utils/blob/master/LICENSE)

git-utils
=========

`git-utils` contains the following utilities:

  * `git-outgoing`

`git-outgoing` provides the following features:

  * Check whether a repository has changesets to push.
  * List the changesets to push.
  * Detect whether a branch has no remote configured.

Prerequisites
-------------

`git-utils` requires the following programs to be present on the `${PATH}`:

  * `zsh`
  * `git`

Getting git-utils
-----------------

A user who whishes to build this package should get a
[release tarball][release].  A release tarball contains everything a user needs
to build the package on his system, following the instructions detailed in the
Installation section below and the `INSTALL` file.

A developer who wishes to modify this package should get the sources (either
from a source tarball or cloning the repository) and have the GNU Build System
installed on his machine.  Please read `README.gnu-build-system` to get further
details about how to bootstrap this package from sources on your machine.

Getting a copy of the source repository is not recommended unless you are a
developer, you have the GNU Build System installed on your machine, and you know
how to bootstrap it on the sources.

[release]: https://github.com/emcrisostomo/git-utils/releases

Installation
------------

See the `INSTALL` file for detailed information about how to configure and
install this package.

Usage
-----

git-outgoing
------------

The syntax to invoke `git-outgoing` is the following:

    $ git-outgoing (options)* (path)*

The available options are:

  * `-h, --help`: to print a usage message.
  * `-v, --verbose`: to print the summary of the outgoing changesets.
  * `--version`: to print the program version.

`path` is the root path of git repository.  If no path is given, `.` is used.

Examples
--------

The following command prints the name of the repositories that have changesets
that have not been pushed:

    $ git-outgoing repo0 ... repon
    repo0
    repo3
    repo7

The following command prints the name of the repositories that have changesets
that have not been pushed and the summary of those changesets:

    $ git-outgoing repo0 ... repon
    repo0
      * 3d22cdc Update po and pot files
      * 131e20d Update C API

Bug Reports
-----------

Bug reports can be sent directly to the authors.

-----

Copyright (c) 2016 Enrico M. Crisostomo

This program is free software; you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation; either version 3, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see <http://www.gnu.org/licenses/>.
