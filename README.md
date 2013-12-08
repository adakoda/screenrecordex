# screenrecordex
A screenrecordex is clone of screenrecord command. It can support 60 minutes recording.

## Download
See http://adakoda.github.io/screenrecordex/

## Install
To install the screenrecordex from the command line, type the following:

`$ adb push screenrecordex /data/local/tmp`

`$ adb shell chmod 755 /data/local/tmp/screenrecordex`

## Run
To use the screenrecordex from the command line, type the following:

`$ adb shell /data/local/tmp/screenrecordex /sdcard/output.mp4`

Stop the screen recording by pressing Ctrl-C, otherwise the recording stops automatically at 60 minutes or the time limit set by --time-limit.
After recording you can download the file from device using adb pull command.

`adb pull /sdcard/output.mp4 .`
