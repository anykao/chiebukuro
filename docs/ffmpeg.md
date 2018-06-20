https://trac.ffmpeg.org/wiki/Concatenate

- `ffmpeg -f concat -safe 0 -i mylist.txt -c copy output`
- `ffmpeg -i <m3u8-url> -c copy -bsf:a aac_adtstoasc output.mp4`

[ffmpeg---command-line](https://github.com/leandromoreira/ffmpeg-libav-tutorial#ffmpeg---command-line)
