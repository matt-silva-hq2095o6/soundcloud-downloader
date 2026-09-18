# soundcloud-downloader

I built this because I wanted a simple command-line utility to download tracks from SoundCloud and get them properly tagged (including album art) without needing ffmpeg installed. It handles both direct progressive MP3 streams and HLS streams by downloading and stitching the TS chunks together directly.

## Installation

Make sure you have Python 3.8+ installed. Clone this repository and install the dependencies:

```cmd
pip install -r requirements.txt
```

## Usage

Run the script with the URL of the SoundCloud track you want to download:

```cmd
python scdl.py https://soundcloud.com/artist/track-name
```

By default, it downloads the track to your current directory using the artist and title for the filename. You can customize the output destination using the `-o` or `--output` argument:

```cmd
python scdl.py https://soundcloud.com/artist/track-name -o "D:\Music\MyTrack.mp3"
```

<!-- refreshed: 2026-09-18 -->
