# MicroCanvas PixelData
JavaScript library for handling different pixeldata formats and creating easing
the creation of monochrome pixelart for embedded devices's displays, such as the
[Arduboy](//github.com/arduboy/arduboy) Arduino-based gaming device and others.

The library is an integral part of the [MicroCanvas HTML5 game framework](
  https://github.com/clouduboy/microcanvas).

## What is a PIF?
PIF is short for `P`ixeldata `I`mage `F`ormat, a plain-text-based intermediary
format to facilitate the creation and sharing of low-resolution, monochrome
image data.

These images are most frequently used in tiny, DIY LCD/LED/OLED displays in
conjunction with small embedded hardware. Creating such images should be
straightforward, but is hindered by the missing simple tooling and the
output requirement of a non-trivial binary pixelformat.

## How to use?
Try the [Sprite Explorer](
  http://clouduboy.github.io/microcanvas-pixeldata/explorer/
) to see some examples! You can modify the examples live, too,
and explore the format by experimenting. You can also use the Explorer to
export a PIF sprite into any of the supported output formats (export code for
Arduino, or regular image formats like PNG, or even SVG!), and to transform
regular PNG/GIF/BMP etc. images into PixelSprites (import).


# License

> This software is licensed under the Apache License, version 2 ("ALv2"), quoted below.
>
> Copyright 2018 István Szmozsánszky, Clouduboy <https://clouduboy.org/>
>
> Licensed under the Apache License, Version 2.0 (the "License");
> you may not use this file except in compliance with the License.
> You may obtain a copy of the License at
>
> http://www.apache.org/licenses/LICENSE-2.0
>
> Unless required by applicable law or agreed to in writing, software
> distributed under the License is distributed on an "AS IS" BASIS,
> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
> See the License for the specific language governing permissions and
> limitations under the License.


# Changelog
- 0.4.1 (2017.07.17) node.js interop fix
  - fix `require()`-s for node apps using the module
  - add updated README with usage help
- 0.4.0 (2017.07.11) Migrated to new URL
  - refactor rename library to `microcanvas-pixeldata`
  - license is now *MIT*
- 0.3.2 (2017.07.10) Experimental SVG representation
  - add `.svg` PIF representation
- 0.3.1 (2017.07.10) Color handling fixes
  - fix `detectPalette()` 3-hex color parsing
  - expose more utilities on `PixelData.util`
- 0.3.0 (2017.06.18) Color/RGBA & loader fixes
  - add import (clone) from `PixelData` object
  - add `rgba2bitmap()` RGBA loader
  - fix `loadPif()` input fault tolerance
- 0.2.5 (2017.03.16) Experimental 8/16 bit colors
  - add experimental 8/16 bit color support
  - add bit depth support for `.c()`
  - add `.b3g3r2` & `.b5g6r5` PIF representations
- 0.2.4 (2017.03.12) Experimental grayscale
  - add experimental color-to-grayscale transformation
  - add color palette metadata handling
  - fix multiframe support
- 0.2.3 (2017.03.07) PixelData byte serialization fix
  - fix `bitmap2bytes()`
- 0.2.2 (2017.03.06) PixelData export fix
  - fix `bitmap2pif()`
- 0.2.1 (2017.03.04) Fixes for use in microcanvas+compiler
  - fix multiframe support
  - add `.rgba()` palette override
- 0.2.0 (2017.03.04) Overhaul, color palette support
  - refactor PIF/C code parsing
  - refactor meta/dimension detection
  - fix PIF generation
  - fix multiframe support
- 0.1.5 (2016.07.17) Fix bitmap loading
  - fix multiframe bitmap loading
- 0.1.4 (2016.07.13) Frames support
  - add `.frames` support
- 0.1.3 (2016.02.18) Fix dimensions heuristics
  - fix heuristics of guessing pixelsprite dimensions
- 0.1.2 (2016.02.07) RGBA support
  - add `bitmapToRgba()` conversion
  - add `.rgba` output format
- 0.1.1 (2015.05.03) BMP-import support for
  - support for loading BMP bitmaps (1bit,24bit,32bit)
- 0.1.0 (2015.05.02) Initial release
