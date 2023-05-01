Burn Captions
=============

This program is loosely based on [mitmul's Burn Captions](https://github.com/mitmul/burn-captions) repository which "[burns] a given SRT file into a video." This version uses moviepy instead of the ffmpeg writer. It still uses imageio to read in the frames of the movie. It adds captions from the SRT file and writes out the frames (sans audio) to a new mp4 file.

## Requirements

Please install required packages by the following command:

```bash
conda install -c conda-forge moviepy
pip install pycaption
 ```

## Usage

```bash
usage: burn.py [-h] [--video VIDEO] [--srt SRT] [--font FONT]
               [--font-size FONT_SIZE] [--bottom-space BOTTOM_SPACE]
               [--skip-first]

optional arguments:
  -h, --help            show this help message and exit
  --video VIDEO
  --srt SRT
  --font FONT
  --font-size FONT_SIZE
  --bottom-space BOTTOM_SPACE
  --skip-first
```

### Example

```bash
python burn.py \
--video sample.mp4 \
--srt sample.srt
```
