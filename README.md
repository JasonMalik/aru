### Features
Android Reverse Utility is a tool that allows you to decompile and rebuild apk.
The program is pretty straight forward and it's made in order to speed up the apk decompile / rebuild process.

ARU it's based on:
- [apktools](https://ibotpeaches.github.io/Apktool/);
- jarsigner;
- [zipalign](https://developer.android.com/studio/releases/platform-tools).

##Installation
```bash
git clone https://github.com/JasonMalik/aru.git
cd aru
./ aru -h
```
All configs are located in the file *config.json*.
All the dependencies required by the program (except for java-sdk) are located inside the *tools* directory, however you can alway re download them using:
```bash
./install
```

##Usage
```bash
usage: aru [-h] (-d DECOMPILE | -b BUILD | -x DEX) [-o OUTPUT] [-v]

Android Reverse Utility

optional arguments:
  -h, --help            show this help message and exit
  -d DECOMPILE, --decompile DECOMPILE
                        Decompile apk
  -b BUILD, --build BUILD
                        Build a source folder into apk
  -x DEX, --dex DEX     Extract all dex
  -o OUTPUT, --output OUTPUT
                        Output filename
  -v, --verbose         Output additional information during the process
```
