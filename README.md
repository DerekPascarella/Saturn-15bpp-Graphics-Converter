# Saturn 15bpp Graphics Converter
A utility to convert between SEGA Saturn 15bpp graphic format and bitmaps.

After dumping 15bpp graphics from a SEGA Saturn game and identifying its dimensions, `15bpp-2-bmp` can be used to convert said graphic data to a bitmap for editing. After editing the bitmap, it can be converted back to its original 15bpp graphic format using `bmp-2-15bpp`.

## Current Version
Saturn 15bpp Graphics Converter is currently at version [1.0](https://github.com/DerekPascarella/Saturn-15bpp-Graphics-Converter/releases/download/1.0/Saturn.15bpp.Graphics.Converter.v1.0.zip).

## Usage
Note that the output filename of `15bpp-2-bmp` will be the input filename with the `.BMP` extension appended (e.g., an input file named `TEX.BIN` will produce `TEX.BIN.BMP`).
```
15bpp-2-bmp <15BPP_FILE> <WIDTH> <HEIGHT>
```
Note that the output filename of `bmp-2-15bpp` will be the input filename with the `.BMP` extension removed (e.g., an input file named `TEX.BIN.BMP` will produce `TEX.BIN`).
```
bmp-2-15bpp <BITMAP_FILE> <WIDTH> <HEIGHT>
```

## Example Usage
Convert a 320x224 15bpp graphic file named `TEX.BIN` to bitmap.
```
15bpp-2-bmp TEX.BIN 320 224
```
Convert a 320x224 bitmap named `TEX.BIN.BMP` to 15bpp graphic format.
```
bmp-2-15bpp TEX.BIN.BMP 320 224
```

## Tutorial
[Malenko](https://segaxtreme.net/members/malenko.22808/) published a fantastic tutorial on the usage of this tool on the [SegaXtreme](https://segaxtreme.net) forums. Click the preview screenshot below to access it.

[![Tutorial Screenshot](https://github.com/DerekPascarella/Saturn-15bpp-Graphics-Converter/blob/main/tutorial.png?raw=true)](https://segaxtreme.net/threads/saturn-15bpp-tool-tutorial.25687/)
