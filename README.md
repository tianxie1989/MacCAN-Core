### MacCAN - USB User-Space Driver for CAN Interfaces under macOS&reg;

_Copyright &copy; 2012-2020  Uwe Vogt, UV Software, Berlin (info@mac-can.com)_

Version $Id$

# Running CAN and CAN FD on a Mac&reg;

_Running CAN and CAN FD on a Mac_ is the mission of the MacCAN project.
The MacCAN-Core repo is not aimed at building a driver or a library.
It holds the source code of an abstraction (or better of a wrapper) of Apple´s IOUsbKit to create USB user-space drivers for CAN interfaces from various vendors under macOS.

## A Stupid Question

I´ve been working with the CAN bus since the late 1990th, mainly on microcontroller
applications (CANopen&reg;, SAE J1939, ISO-TP, UDS, etc.), but also on PC; see https://www.uv-software.com/wordpress.

I tend to ask myself sometimes some stupid questions like "Is it possible to ...?".
In 2010 I asked a well known search engine if it is possible to run CAN on a Mac.
I only found the request of a student, who had to do a semester work with CAN bus.
But that poor boy only owned a Mac.

## Servicing the Milky Way and Beyond

___MacCAN, macOS Library for PCAN-USB interfaces and more.___

In 2012 I´ve started with the development of a macOS (a.k.a. OS X) user-space driver for my PEAK CAN to USB dongle.
Many thanks to Uwe Wilhelm, CEO of PEAK-System Technik GmbH, who had supported me with technical informations and several hardware.

### The PCBUSB Library

The _PCBUSB_ library realizes a USB user-space driver under macOS for PCAN&reg; USB interfaces from PEAK-System Technik, Darmstadt; see https://www.mac-can.com.

It supports up to 8 PCAN-USB and PCAN-USB FD devices.
The library offers an easy to use API to read received CAN messages from a 64K message queue and to transmit CAN messages.
Standard CAN frames (11-bit identifier) as well as extended CAN frames (29-bit identifier) are supported.
The PCAN-USB FD device can be operated in CAN 2.0 and CAN FD mode.

The library comes with an Objective-C wrapper and a demo App; see https://youtu.be/v0U_WN7s3ao </br>
Furthermore, it can be used with the Qt&reg; Serial Bus API on a Mac; see https://doc.qt.io/qt-5/qtserialbus-index.html

The PCBUSB library is closed source, please note the copyright and license agreements.

### TouCAN USB Interfaces from Rusoku

In 2020 I´ve receive the request from Gediminas Simanskis, CEO of Rusoku technologijos UAB, Lithuania, to roll out the MacCAN project to their TouCAN USB devices.
For the products and services they offer see https://www.rusoku.com.

And in JL's words, "Make it so!"; see https://github.com/mac-can/TouCAN-USB

## HowTo

[To Be Continued]

## This and That

### SVN Repo

The MacCAN-Core sources are maintained in an SVN repo to synchronized them between the different MacCAN child repos via Git SVN bridge.
Git submodules or subtrees could be an alternative way for the future.

### License

MacCAN-Core is free software: you can redistribute it and/or modify
it under the terms of the GNU Lesser General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

MacCAN-Core is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License
along with MacCAN-Core.  If not, see <http://www.gnu.org/licenses/>.

### Trademarks

Mac and macOS are trademarks of Apple Inc., registered in the U.S. and other countries. </br>
PCAN is a registered trademark of PEAK-System Technik GmbH, Darmstadt, Germany. </br>
Qt is a registered trademark of The Qt Company Ltd. and its subsidiaries.

### Contact

Uwe Vogt </br>
UV Software </br>
Chausseestrasse 33a </br>
10115 Berlin </br>
Allemagne

E-Mail: mailto://info@mac.can.com </br>
Internet: https://www.mac-can.com

#### *Happy Engineering!*
