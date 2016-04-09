# Crunchyget

Crunchyget is a script that allows you to easily download videos from
Crunchyroll. It uses [youtube-dl][1] to download the videos, and can
automatically rename them and convert them to MP4 format using [ffmpeg][2]. It
can download and convert multiple videos at the same time to the same directory,
without facing any problems due to multiple instances.

Crunchyget is currently available for Linux and OS X, but it could be ported to
Windows if there is high demand.

Dependencies: [youtube-dl][1], [ffmpeg][2], [perl-rename][3]

## Quick setup

Open a terminal and run the following:

    curl -o setup https://raw.githubusercontent.com/tech4david/crunchyget/master/setup
    sh setup

## Subtitles

Subtitles will be saved to the '.subtitles' directory (folder) where the video
has been downloaded to. This directory will be created if it does not yet exist.
Because it begins with a dot, it will be hidden by default. To enable automatic
subtitle detection on VLC media player, do the following:

1. Open Tools » Preferences
2. Under 'Show settings', click 'All'
3. Scroll to the bottom of the sidebar and click 'Subtitles / OSD'
4. In the box 'Subtitle auto-detection paths', append `, ./.subtitles`
5. Click 'Save'

## Disclaimer

This program is for personal use only, and comes with no warranty. Use at your
own risk!

[1]: https://rg3.github.io/youtube-dl/
[2]: https://www.ffmpeg.org/
[3]: http://search.cpan.org/~rmbarker/File-Rename/rename.PL
