# intervallo

Generate picture slideshows similar to
[RAI](https://en.wikipedia.org/wiki/RAI)'s iconic
["Intervallo"](https://it.wikipedia.org/wiki/Intervallo_(televisione))

## Usage:

```
$ intervallo --help
usage: intervallo [-h] [--font file.ttf] [--audio file.mp3] [--duration sec]
                  imgfile [imgfile ...]

Create an Intervallo RAI out of a collection of images.

positional arguments:
  imgfile           input image files

optional arguments:
  -h, --help        show this help message and exit
  --font file.ttf   Font to use for subtitles
  --audio file.mp3  Audio track
  --duration sec    Time for each image in seconds
```

For example:

```
./intervallo --font DejaVuSerif.ttf --audio Paradisi-Toccata.mp3 *.jpg
```

The images are captioned with their file name, without extension. You may want
to rename the image files to have nice descriptive names.

Alternatively, you can create a `foo.jpg.txt` file for a `foo.jpg` image, so
you can have multiline captions.

See [here](https://www.jamendo.com/track/708643/p-d-paradisi-toccata) for a
suitable audio.
[archive.org](https://archive.org/details/IntervalloRai-Paradisi) has a track
that is very close to the original, but I did not see information about its
license.

## Examples

Original versions:
<https://www.youtube.com/playlist?list=PLY8ZnKIqYfqb8VZaeLHSDhNLziwjeT0-H>

For an '80s style intervallo like [this](https://www.youtube.com/watch?v=_ACoU8fRyEw&list=PLY8ZnKIqYfqb8VZaeLHSDhNLziwjeT0-H&index=2):
```
./intervallo --audio Emilio_Antonucci_-_P.D._PARADISI__TOCCATA.mp3 *.jpg
```

Other fonts to try:

 * [Latin Modern Roman demi](https://www.fontsquirrel.com/fonts/Latin-Modern-Roman) (`apt install fonts-lmodern` in Debian, then use `/usr/share/texmf/fonts/opentype/public/lm/lmromandemi10-regular.otf`)
