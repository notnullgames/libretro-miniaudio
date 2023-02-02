# audio_no_callback
This sample demonstrates how to generate sound using libretro API with no audio callback.

> Experiment abandoned in favor of [soloud](https://github.com/notnullgames/libretro-soloud)

What this means is that libretro's audio callback function has to be called inside retro_run
at least once per run.

The audio samplerate in this sample is set to 4800KHz, sound is 16-bit mono.

I am trying to get ot working with [miniaudio](https://miniaud.io/)


## Building
To compile, you will need a C compiler and assorted toolchain installed.

	make

## Running

```
# mac
/Applications/RetroArch.app/Contents/MacOS/RetroArch -L testaudio_no_callback_libretro.dylib

# windows
retroArch -L testaudio_no_callback_libretro.dll

# linux
retroArch -L testaudio_no_callback_libretro.so
```
