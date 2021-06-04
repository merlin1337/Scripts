# Scripts
Various helper scripts and stuff. Pretty much Windows only

- [Scripts](#scripts)
  - [WebP conversion](#webp-conversion)
    - [webp2gif.bat](#webp2gifbat)
    - [webp2gifski.bat](#webp2gifskibat)
    - [webp2mp4.bat](#webp2mp4bat)
  - [Zip and upload/move directory](#zip-and-uploadmove-directory)
    - [deploy_MEGA.bat](#deploy_megabat)

## WebP conversion

### webp2gif.bat
Creates a converted GIF next to input file. [Relevant FFmpeg settings](http://ffmpeg.org/ffmpeg-filters.html#palettegen-1) can be easily changed

**Requires:**
[ffmpeg](https://www.ffmpeg.org/) and
[libwebp](https://developers.google.com/speed/webp/download) (anim_dump, webpinfo)

### webp2gifski.bat
Creates a converted, high-quality (and huge) GIF next to input file

**Requires:**
[merlin1337/gifski](https://github.com/merlin1337/gifski) (Fork) and
[libwebp](https://developers.google.com/speed/webp/download) (anim_dump, webpinfo)

### webp2mp4.bat
Creates a converted MP4 next to input file. Very compact and good quality but apparently not suited for having looping video in WPF (which is also the reason why I ended up writing THREE different webp scripts...)

**Requires:**
[ffmpeg](https://www.ffmpeg.org/) and
[libwebp](https://developers.google.com/speed/webp/download) (anim_dump, webpinfo)

## Zip and upload/move directory

### deploy_MEGA.bat
Zips a directory, uploads archive to MEGA and moves it somewhere.

**Requires:**
[MEGAcmd](https://mega.nz/cmd),
[7z](https://7-zip.org/) and
[7z LZMA SDK](https://7-zip.org/sdk.html) (7z.sfx)\
**Usage:**
```deploy_MEGA <directory> <zip name> <MEGA path> <local path>```\
**Usage:**
```deploy_MEGA "C:\MyProject\bin\Release" MyProject-Release "/Uploaded Packages" "D:\Local Packages"```