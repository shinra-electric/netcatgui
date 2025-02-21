> [!Note]
> This fork of NetcatGUI is intended for macOS<br>
> There are no Linux/Windows changes, so it should still work for those platforms<br>
> The following readme is from the original project except for the macOS instructions<br>


# About NetcatGUI

NetcatGUI is a simple gui program that is set to emulate the popular
network "swiss army knife" tool called netcat(nc) using an easy to use
graphical user interface and cross platform mentality.
There are easy keyboard shortcuts for almost every operation of NetcatGUI
in order to achieve maximum efficiency. If you get used to them(they're 
pretty obvious) you will feel as close as you can to a console despite
of using a gui.


NetcatGUI is written in Qt, thus it supports Linux, Mac OS X, BSD and 
Windows out of the box.


## Supported Platforms

The binary packages support the following platforms:

- Windows
- Linux
- macOS (I don't have a Mac yet, thus I can't make an official build)

Building the sources requires Qt 4.7.0 or later.

## Compiling on macOS

- Install the Xcode Command-line Tools with `xcode-select --install`
- Install [Homebrew](https://brew.sh) 
- Install Qt with `brew install qt`
- Clone this repo and cd into it
- Use the command `qmake netcatgui.pro && make`
- If it compiles successfully you should see the NatcatGUI app bundle in the `build` directory

## Compiling on Unix/Linux and Windows

Prerequisites:
   - Qt 4.7.0 or later
   - On Linux you have two choices for installing the Qt SDK:
        1. Install Qt 4.7.0 or later using your distribution's
            package manager. The minimum libraries you need are
            libqt4-core, libqt4-gui and libqt4-dev. Besides that
            you will need qt4-qmake for qmake and g++/libstdc++5, 
            though these should be automatically installed as 
            dependencies to libqt*.
            For e.g. on debian you can:
            apt-get install libqt4-core libqt4-gui libqt4-dev
            and say yes to the dependencies and you get everything
            you need.
        2. Install the latest official Qt SDK available at:
            http://qt.nokia.com/downloads/
   - On Windows:
     -  MinGW 4.4 or later, Visual Studio 2008 or later
     -  jom
     The Qt SDK provides you with most of the required software.
     Grab the official Qt SDK from http://qt.nokia.com/downloads/
	 -  open an instance of Qt SDK Command Prompt

Building:

cd ncgui/
qmake netcatqui.pro
make (or mingw32-make or nmake or jom, depending on your platform)

Installing(on *NIX):
make install //not implemented

To clean the build directory:
make clean && make distclean

# Documentation

- this file
- the home page: http://shinnok.com/projects.php

## Usage

Nothing special, just run the program and browse around. There's nothing you 
can break or something like that. :-)

I'll list a couple of useful keyboard shortcuts you can use with NetcatGUI(you can view all of them in the menus or hover above buttons):

    -Ctrl^q : quit the application
    -Ctrl^t : new connect tab
    -Ctrl^l : new listen tab
    -Ctrl^w : close tab
    -Ctrl^Tab : next open tab
    -Ctrl^Shift^Tab : previous open tab
    -Shift^Enter : New line in the input box
    -Ctrl^o : start connect or listen, depending on the current tab
    -Ctrl^d : stop connect if on connect tab, stop connection if on listen tab
              and a connection is made or stop listening respectively
    -Enter/Return : send message

## Reporting bugs

Report bugs using Github issues or send directly to admin<at>shinnok<dot>com.

## Third-party components


NetcatGUI uses icons from the iconpack Silk icon set 1.3 by Mark James.
http://www.famfamfam.com/lab/icons/silk/

========================================================================

Copyright (C) Shinnok <Teodor Mircea Ionita> NetcatGUI

This software distribution is licensed under the GNU General Public License
version 2 (GPL-2.0). For details see COPYING dist file.
