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
