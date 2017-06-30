# waifu2x-Video Enhancer
Just as waifu2x works to enhance resolution and edit "Anime-Style Art" (images), waifu2x-video is a batch script which works the same way but for VIDEOS!

### Softwares used:  
It uses following open source softwares:
* `waifu2x-caffe`
	- [Source](https://github.com/lltcggie/waifu2x-caffe)
	- [Release](https://github.com/lltcggie/waifu2x-caffe/releases)
* `ffmpeg (including ffmprobe)`
	- [Source](https://github.com/FFmpeg/FFmpeg)
	- [Release](https://ffmpeg.zeranoe.com/builds/win32/static/)

### Instructions to setting up for use:
This script changes resolution of videos. Resolution of videos can be increased or decreased. Frames are optimized by using waifu2x-caffe, so you can perform all optimizations available for cui version of waifu2x-caffe (see its readme for details).

#### Softwares you need to download:
* `ffmpeg.exe & ffprobe.exe` [Direct link to ffmpeg-20170130](https://ffmpeg.zeranoe.com/builds/win32/static/ffmpeg-20170130-cba4f0e-win32-static.zip)
* `waifu2x-caffe` [Direct link to v1.1.8.3](https://github.com/lltcggie/waifu2x-caffe/releases/download/1.1.8.3/waifu2x-caffe.zip)  

##### Setting up:
1. Download all 3 softwares. ffmpeg.exe and ffmprobe.exe will be in same zip.

2. Extract ffmpeg and ffprobe

3. After install.bat runs successfully, you can use "Optimize Video Resolution.bat". It can be used from
anywhere.
