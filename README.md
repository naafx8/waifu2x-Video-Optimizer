# waifu2x-Video Optimizer
Just as waifu2x works to enhance resolution and edit "Anime-Style Art" (images), waifu2x-video is a batch script which works the same way but for VIDEOS using waifu2x!

## Please Note
* This script will only run in Windows OS. Although you can make bash version of this batch script yourself for Linux or Mac.
* This script converts each frame using waift2x-caffe. Depending on number of total frames and time required to process each frame, this script can take lots of hard disk space and lots of CPU/GPU memory. **This may cause some problems on CPU/GPU** bause this script is not meant to be used on low specs PCs. First try using this script on a small sample video of 10 to 20 seconds long while also keeping an eye on usage/temperature status of CPU and GPU using `MSI After Burner` or `Open Hardware Monitor`. *I won't be responsible for any harm to your PC*.
* waifu2x-caffe has many cli options for optimizing image. Read [README.md](https://github.com/lltcggie/waifu2x-caffe/blob/master/README.md) (You can translate it using Google Translate). Feel free to edit the script to change optimization settings.

### Softwares used:  
It uses following open source softwares:
* `waifu2x-caffe`
	- [Source](https://github.com/lltcggie/waifu2x-caffe)
	- [Release](https://github.com/lltcggie/waifu2x-caffe/releases)
* `ffmpeg (including ffmprobe)`
	- [Source](https://github.com/FFmpeg/FFmpeg)
	- [Release](https://ffmpeg.zeranoe.com/builds/win32/static/)

### Instructions to setting up for use:
This script changes resolution of videos. Resolution of videos can be increased or decreased. Frames are optimized by using waifu2x-caffe, so you can perform all optimizations available for cli version of waifu2x-caffe (see its readme for details).

#### Softwares you need to download:
* `ffmpeg.exe & ffprobe.exe` [Click here to direct download ffmpeg-20170130](https://ffmpeg.zeranoe.com/builds/win32/static/ffmpeg-20170130-cba4f0e-win32-static.zip)
* `waifu2x-caffe` [Click here to direct download v1.1.8.3](https://github.com/lltcggie/waifu2x-caffe/releases/download/1.1.8.3/waifu2x-caffe.zip)  

##### Setting up:
1. Extract `ffmpeg-20******-win32-static.zip` and copy ffmpeg.exe and ffprobe.exe to `C:\Windows\System32`. This way the script will be able to access these both programs from anywhere easily.  
2. Extract `waifu2x-caffe.zip`. There will be a folder named "waifu2x-caffe". Copy this folder to `"C:\Program Files"`. So `waifu2x-caffe-cui.exe` will be in `"C:\Program Files\waifu2x-caffe\"`
3. Now you need to add path of `waifu2x-caffe-cui.exe` in a system variable. Open `CMD` and type the following command:
> setx waifu2x "\\"C:\Program Files\waifu2x-caffe\waifu2x-caffe-cui.exe\\""  
You are all set now. Open `waifu2x-Video-Optimizer.bat`, paste the path of video and select video resolution of result video.
