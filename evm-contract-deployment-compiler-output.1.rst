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


===============================================
evm-contract-deployment-compiler-output
===============================================

-----------------------------------------------------------------------------------
Ethereum Virtual Machine (EVM) contract deployment compiler output discover tool
-----------------------------------------------------------------------------------
:Version: evm-contract-deployment-compiler-output |version|
:Manual section: 1


Synopsis
========

evm-contract-deployment-compiler-output *[options]* *target-contract*


Description
===========

Returns an EVM network's contract deployment compiler output
(HardHat json file).


Networks
=========

All those supported by
'evm-chains-info' as
well as direct RPC addresses.


Options
=======

-n network, --network network                      EVM network name.

-i network-id, --chain-id number                   EVM network id.

-A, --networks-all                                 Returns address for all
                                                   available networks.

-a target-app, --target-app app                    Application whose target
                                                   contract is part of.

-V contract-version, --contract-version version    Contract version.

-u, --user-defined                                 Returns contract address for
                                                   user-defined file system
                                                   deployment instead of the
                                                   system one.

-d directory, --deployments-dir dir                Specify contracts deployments
                                                   directory path.

-f format, --configuration-format format           Specify contracts deployments
                                                   configuration format. It can be
                                                   'bash' or 'json'.

-h, --help                                         Displays help.

-c, --color                                        Enable color output

-v, --verbose                                      Enable verbose output


Bugs
====

https://github.com/themartiancompany/evm-contracts-tools/-/issues


Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.


See also
========

* evm-contract-call
* evm-contract-deployment-abi
* evm-contract-deployment-address
* evm-contract-deployment-bytecode
* evm-contract-deployment-networks
* evm-contract-deployment-versions
* evm-contract-deployments-dir
* evm-contracts-abi-get
* evm-wallet

.. include:: variables.rst
