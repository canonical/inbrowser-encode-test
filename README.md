# inbrowser-encode-test
Testing video encoding in a browser.

This web-page will create a procedural animation that is encoded as video.

# Usage

This test was specifically created to check if your browser will use the GPU to help with the encoding, so called Hardware-Accelerated-Encoding.
To perform this test, it is recommended to have a GPU monitor running on your desktop.
You can use e.g.
[intel_gpu_top](https://manpages.ubuntu.com/manpages/kinetic/man1/intel_gpu_top.1.html)
if you use an Intel GPU.
Run as root `$ sudo intel_gpu_top` to check the Video usage.


# Options

Before encoding, select which encoder you want to use.
Note that at the time of writing, not all browsers support all formats, and you may get an error when you encode.
I've found that both Firefox and Chromium are happy to do VP9, which is the default encoder.

After encoding, you can either download the resulting video, or play it in the video-player at the bottom of the page.

# Limitations

Many things are hard-coded at the moment:
 * video resolution set to 1280x720.
 * video FPS set to 60Hz.
 * video length set to 300 frames.

# Author

Bram Stolk (bram.stolk@canonical.com)

