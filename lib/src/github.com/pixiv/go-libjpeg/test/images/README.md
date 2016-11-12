Example Images
==============

This directory contains example JPEG files and PNG source files.

## Photos by Author

These images are taken by [Shunsuke Michii](https://github.com/harukasan).
These photos are licensed under the Creative Commons Attribution 3.0.
You can also use these images under the same as [go-libjpeg's license](../LICENSE).

#### cosmos.png

The cosmos taken in Nokono-shima (Nokono Island), Fukuoka, JAPAN.

![cosmos.png](cosmos.png)

JPEG file is generated by following command:

```sh
$ convert -quality 90 -sampling-factor 4:2:0 ./cosmos.png ./cosmos.jpg
```

#### kinkaku.png

Kinkaku taken in Kyoto, JAPAN.

![kinkaku.png](kinkaku.png)

JPEG file is generated by following command:

```sh
$ convert -quality 90 -sampling-factor 4:2:0 ./kinkaku.png ./kinkaku.jpg
```

## Checkerboard

Blue and Red Checkerboards in each subsampling factor.

Each images are converted by following commands:

```
$ convert checkerboard.png -sampling-factor 4:4:4 -quality 100 ./checkerboard_444.jpg
$ convert checkerboard.png -sampling-factor 4:4:0 -quality 100 ./checkerboard_440.jpg
$ convert checkerboard.png -sampling-factor 4:2:2 -quality 100 ./checkerboard_422.jpg
$ convert checkerboard.png -sampling-factor 4:2:0 -quality 100 ./checkerboard_420.jpg
```

## testdata from Go Standard library

The images that included in the [testdata](./testdata/) directory are ported from [golang/go](https://github.com/golang/go).

Original files are found here: https://github.com/golang/go/tree/master/src/image/testdata

```
Copyright (c) 2012 The Go Authors. All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

   * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
   * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
   * Neither the name of Google Inc. nor the names of its
contributors may be used to endorse or promote products derived from
this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```