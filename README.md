IFR Extractor LS v0.3
=======================

Utility to extract the internal forms representation from both EFI and UEFI drivers/applications into human readable text file.

A fork of <a href="https://github.com/donovan6000/Universal-IFR-Extractor">Donovan6000's project</a> with bugfixes and additions.

Original code by Donovan6000, rewritten UEFI.cpp by TomRus88, fixes and additions by DeathBringer, Fernando Rodriguez and Seth Stahlman.

This fork provides linux prebuit binary. If you want to build it by yourself, execute the following:

`cd Downloads; sudo apt install git cmake; git clone https://github.com/macos86/Universal-IFR-Extractor.git; mkdir build; pushd build; cmake ..; make`

## Usage

Extract the Setup.bin PE32 Image section clicking on "Extract Image" when you are using UEFITool (after searching for "CFG Lock") - then save the file as .bin

After you've done that, use ifrextractor in order to be able to read the .bin file in a .txt format

`./ifrextract Setup.bin Setup.txt`
