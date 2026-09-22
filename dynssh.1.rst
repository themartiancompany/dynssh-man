..
   SPDX-License-Identifier: AGPL-3.0-or-later

   -------------------------------------------------------
   Copyright © 2024, 2025, 2026
               Pellegrino Prevete

   All rights reserved
   -------------------------------------------------------

   This program is free software: you can redistribute it
   and/or modify it under the terms of the
   GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the
   License, or (at your option) any later version.

   This program is distributed in the hope that it will
   be useful, but WITHOUT ANY WARRANTY; without even the
   implied warranty of MERCHANTABILITY or FITNESS FOR A
   PARTICULAR PURPOSE.
   See the GNU Affero General Public License
   for more details.

   You should have received a copy of the
   GNU Affero General Public License
   along with this program.
   If not, see <https://www.gnu.org/licenses/>.


========================
dynssh
========================

--------------------------------------------------------------
SSH client with host address auto-detection
--------------------------------------------------------------
:Version: dynssh |version|
:Manual section: 1


Synopsis
========

dynssh *[options]* -- *[ssh-options]* *[ssh-args]*


Description
===========

SSH client which relies on *hotspot-resolver*
for determining the host address when connected
on networks which change subnet often, like
for example recent Android devices.


Options
=======

-t <target-host>     Specify target host
-a <address>         Specify target address
-d <device>          Specify network device
-u <user>            user to connect to.
-p <port>            Connect through a specific port.
-l <local-port>      Tunnel on given local port
-r <remote-port>     Tunnel on given remote port
-T <proxy-address>   Specify a proxy address
-P <proxy-port>      Specify a proxy port
-C <ssh-path>        Connect using a specific ssh supporting binary
                     (possible values one can use are 'ssh',
                     'autossh', 'rsync').
-m <monitor-port>    Specify monitor port when using autossh


Application options
=====================

-h                   Display help.
-c                   Enable color output
-v                   Enable verbose output


Environment variables
=======================

* *HOTSPOT_RESOLVER_OPTS*

    This variable is read to pass custom options
    to 'hotspot-resolver' (for example the global
    host option '-G').

Bugs
====

https://github.com/themartiancompany/dynssh/-/issues


Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* hotspot-resolver

.. include:: variables.rst
