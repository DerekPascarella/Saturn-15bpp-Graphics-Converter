# Saturn 15bpp Graphics Converter
A utility to convert between SEGA Saturn 15bpp graphics format and bitmap.

After dumping 15bpp graphics from a SEGA Saturn game (typically found in VDP2 RAM) and identifying its dimensions, `15bpp-2-bmp` can be used to convert said graphic data to a bitmap for editing. After editing the bitmap, it can be converted back to its original 15bpp graphics format using `bmp-2-15bpp`.

## Current Version
Saturn 15bpp Graphics Converter is currently at version [1.0](xxxx).

## Usage
Note that the output filename of `15bpp-2-bmp` will be the input filename with the ".BMP" extension appended (e.g., an input file named "TEX.BIN" will produce "TEX.BIN.BMP").
```
bmp-2-15bpp <BITMAP_FILE> <WIDTH> <HEIGHT>
```
Note that the output filename of `bmp-2-15bpp` will be the input filename with the ".BMP" extension removed (e.g., an input file named "TEX.BIN.BMP" will produce "TEX.BIN").
```
15bpp-2-bmp <15BPP_FILE> <WIDTH> <HEIGHT>
```

## Example Usage
Convert a 320x224 15bpp graphics file named "TEXT.BIN" to bitmap:
```
15bpp-2-bmp TEX.BIN 320 224
```
Convert a 320x224 bitmap named "TEX.BIN.BMP" to 15bpp graphics format.
```
bmp-2-15bpp TEX.BIN.BMP 320 224
```
