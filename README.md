> [!Note]
> This fork of [NetcatGUI](https://github.com/shinnok/netcatgui) is intended for macOS<br>
> It should still work for Linux, BSD and Windows, but it is untested<br>
> The following readme is from the original project but has been edited to reflect updates<br>

# About NetcatGUI

NetcatGUI is a simple gui program that is set to emulate the popular netcat(nc) network tool, using an easy-to-use graphical user interface.<br>

There are easy keyboard shortcuts for almost every operation of NetcatGUI in order to achieve maximum efficiency.<br>

NetcatGUI is written using Qt and supports macOS, Linux, BSD and Windows out of the box.

## Compiling on macOS

- Install the Xcode Command-line Tools with `xcode-select --install`
- Install [Homebrew](https://brew.sh) 
- Install Qt with `brew install qt`
- Clone this repo and cd into it
- Use the command `qmake netcatgui.pro && make`
- If it compiles successfully you should see the NatcatGUI app bundle in the `build` directory

## Usage

Here are a few useful keyboard shortcuts you can use with NetcatGUI (you can view all of them in the menus or hover above buttons):

   - Ctrl^q : quit the application
   - Ctrl^t : new connect tab
   - Ctrl^l : new listen tab
   - Ctrl^w : close tab
   - Ctrl^Tab : next open tab
   - Ctrl^Shift^Tab : previous open tab
   - Shift^Enter : New line in the input box
   - Ctrl^o : start connect or listen, depending on the current tab
   - Ctrl^d : stop connect if on connect tab, stop connection if on listen tab and a connection is made or stop listening respectively
   - Enter/Return : send message

