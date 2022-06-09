# showyourself :framed_picture: 

16 color image viewer for the terminal that uses [content aware image resizing](https://github.com/esimov/caire).

## Why

I wanted to develop an image viewer that could be usable from within [`o`](https://github.com/xyproto/o), a small editor/IDE I wrote that targets VT100 compatible terminal emulators.

## Features and limitations

* The content-aware image resizing changes the image, but keeps the most interesting content.
* The palette reduction is done by [`palgen`](https://github.com/xyproto/palgen).

## Comparison

| Original PNG image                    | In a VT100 compatible terminal emulator, using 16 colors |
|---------------------------------------|----------------------------------------------------------|
| <img src=img/grumpycat.png width=512> |            <img src=img/grumpycat16colors.png width=512> |
| <img src=img/archbtw.png width=512>   |              <img src=img/archbtw16colors.png width=512> |
| <img src=img/rt.png width=512>        |                   <img src=img/rt16colors.png width=512> |

The images are changed, but the essence is kept.

## Installation

The `viewpng` utility can be installed with Go 1.17 or later:

    go install github.com/xyproto/showyourself/cmd/viewpng@latest

## General info

* Version: 1.0.0
* License: BSD-3
* Author: Alexander F. Rødseth &lt;xyproto@archlinux.org&gt;
