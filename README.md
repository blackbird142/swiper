# swiper
Live wallpaper engine for Linux systems that support `feh --bg-scale`.

## Preview
![Swiper demo gif](demo.gif)

## Getting started
### Dependencies
Install `feh`, `ffmpeg`, `ffprobe`
### Installation
```
git clone https://github.com/spitmirror/swiper/edit/main/README.md; cd swiper; make
```

### Common usage
No arguments for help menu.
```
$ ./swiper
```
Set mp4 wallpaper with jpg (default) frames, and 1280x720 aspect ratio.
```
$ ./swiper -s ~kruz/298983.mp4 -w 1280 -h 720
```
Set gif wallpaper at 44.2 fps with png frames, apply in daemon mode.
```
$ ./swiper -s 90s-synth.gif -r 442/10 -P -ad
```
Apply currently set wallpaper in daemon mode with frame caching.
```
# ./swiper -adc
```
Set live wallpaper at 15 fps with png frames, apply in daemon mode at 20 playback fps with frame caching.
```
# swiper -s /file.ext -r 15 -w 1280 -h 720 -Pac -p 20`
```

## Authors
* **Spit** - [spitmirror](https://github.com/spitmirror)

## Acknowledgments
This project has been inspired by
* n/a
