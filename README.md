# clitube
A terminal-based and privacy-focused YouTube streamer.

## How does clitube work?
It is very simple : using Invidious' API, we can get a `.json` that contains our search results. The `.json` contains the details of each video that was shown in our search. To play the video, we get the `videoId` and place it in a Invidious instance URL. clitube also gets the `author`, `viewCount` and `title` to display them after the user selects a video.

## What is Invidious?
Invidious is an amazing open-source alternative front-end to YouTube.You can see more details by visiting their [repository](https://github.com/iv-org/invidious).

## Why use Invidious when YouTube has an API that does the same thing?
Unlike YouTube (or any Google service for that matter), Invidious respects the user's privacy, doesn't track the user's activity and it has no ads whatsoever. 

## How to use
Download the script and give it the execute permission by running :
```
bash
chmod +x clitube
```
You can run it from anywhere, but if you want to, you can move it to your `bin` directory:
```
bash
sudo mv clitube /bin/clitube
```
The script doesn't take any arguments, so you can simply run it by calling it.
```
clitube # if moved to /bin
./clitube # if you are using it as a portable script
```
## Preview of clitube
 ![](clitube-preview.gif)
 
## Dependecies
Make sure you have the following dependencies installed :
- mpv

The following usually come with every distro, but make sure they are installed :
- awk
- grep
- curl

## Other notes
By default, mpv will use the highest quality available.
If you want to switch the video quality, you can use the following script
which will allow you to change the video quality on the fly. Link to it :
https://github.com/jgreco/mpv-youtube-quality

# Credits
 - [Andrei Datcu](https://datcuandrei.github.io) : creator of clitube.
 - [Invidious](https://github.com/iv-org/invidious) : creators of the amazing API and private front-end for YT.
 - [mpv](https://mpv.io/) : creators of the player used by clitube.
# License
```
MIT License

Copyright (c) 2021 Andrei Datcu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
