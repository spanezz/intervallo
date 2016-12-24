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

For some audio to use, you can try <https://archive.org/details/IntervalloRai-Paradisi>

## Example

https://www.youtube.com/watch?v=ZCERwjTB4ck