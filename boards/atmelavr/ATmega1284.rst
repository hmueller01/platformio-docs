..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _board_atmelavr_ATmega1284:

ATmega1284
==========

.. contents::

Hardware
--------

Platform :ref:`platform_atmelavr`: Atmel AVR 8-bit MCUs deliver a unique combination of performance, power efficiency and design flexibility. Optimized to speed time to market-and easily adapt to new ones-they are based on the industry's most code-efficient architecture for C and assembly programming

.. list-table::

  * - **Microcontroller**
    - ATMEGA1284
  * - **Frequency**
    - 16MHz
  * - **Flash**
    - 128KB
  * - **RAM**
    - 16KB
  * - **Vendor**
    - `Microchip <https://www.microchip.com/wwwproducts/en/ATmega1284?utm_source=platformio.org&utm_medium=docs>`__


Configuration
-------------

Please use ``ATmega1284`` ID for :ref:`projectconf_env_board` option in :ref:`projectconf`:

.. code-block:: ini

  [env:ATmega1284]
  platform = atmelavr
  board = ATmega1284

You can override default ATmega1284 settings per build environment using
``board_***`` option, where ``***`` is a JSON object path from
board manifest `ATmega1284.json <https://github.com/platformio/platform-atmelavr/blob/master/boards/ATmega1284.json>`_. For example,
``board_build.mcu``, ``board_build.f_cpu``, etc.

.. code-block:: ini

  [env:ATmega1284]
  platform = atmelavr
  board = ATmega1284

  ; change microcontroller
  board_build.mcu = atmega1284

  ; change MCU frequency
  board_build.f_cpu = 16000000L

Debugging
---------

:ref:`piodebug` - "1-click" solution for debugging with a zero configuration.

.. warning::
    You will need to install debug tool drivers depending on your system.
    Please click on compatible debug tool below for the further
    instructions and configuration information.

You can switch between debugging :ref:`debugging_tools` using
:ref:`projectconf_debug_tool` option in :ref:`projectconf`.

ATmega1284 does not have on-board debug probe and **IS NOT READY** for debugging. You will need to use/buy one of external probe listed below.

.. list-table::
  :header-rows:  1

  * - Compatible Tools
    - On-board
    - Default
  * - :ref:`debugging_tool_simavr`
    - 
    - Yes

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_arduino`
      - Arduino Wiring-based Framework allows writing cross-platform software to control devices attached to a wide range of Arduino boards to create all kinds of creative coding, interactive objects, spaces or physical experiences