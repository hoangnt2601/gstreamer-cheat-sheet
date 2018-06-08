# GStreamer command-line cheat sheet

This series of docs provides a cheat sheet for GStreamer on the command-line.

A few Python examples are also [included](python_examples/) for when you need GStreamer to be dynamic (i.e. react to user or some other action).

## Contents

* [Basics](basics.md)
* [Test streams](test_streams.md)
* [RTMP](rtmp.md)
* [Mixing video & audio](mixing.md)
* [Images](images.md)
* [Queues](queues.md)
* [Capturing images](capturing_images.md)
* [Sending to multiple destinations (tee)](tee.md)
* [Sharing and receiving pipelines, including sending/receiving video from shared memory](sharing_and_splitting_pipelines.md)
* [Network transfer](network_transfer.md) (including how to send so that VLC can preview)

## Sources and references

* [Basic command line reference](http://docs.gstreamer.com/display/GstSDK/Basic+tutorial+10%3A+GStreamer+tools)
* [Pipeline examples](https://gstreamer.freedesktop.org/documentation/tools/gst-launch.html#pipeline-examples)
* [List of all Gstreamer plugins](https://gstreamer.freedesktop.org/documentation/plugins.html)
* [Handy elements](https://gstreamer.freedesktop.org/documentation/tutorials/basic/handy-elements.html#uridecodebin)

## Other cheat-sheets

* http://wiki.oz9aec.net/index.php/Gstreamer_cheat_sheet
* https://github.com/xmementoit/gstreamerCheatsheet/blob/master/README.md
* https://gist.github.com/nebgnahz/26a60cd28f671a8b7f522e80e75a9aa5

## Interacting with the GStreamer pipeline

If you want to interact with GStreamer after it's started (e.g. respond to an event, or dynamically change a pipeline), the command-line GStreamer doesn't really cut it. Instead, here are some options:

* *[GStreamer Daemon (gstd)](https://github.com/RidgeRun/gstd-1.x)* - allows setting and updating via a TCP connection
* *[Snowmix](http://snowmix.sourceforge.net/)* - an open-source live video mixer
* *Develop using the GStreamer library*, in either [C](https://gstreamer.freedesktop.org/documentation/application-development/basics/helloworld.html), [Python](https://github.com/GStreamer/gst-python), or [C#/.NET](https://github.com/GStreamer/gstreamer-sharp)

### Python with GStreamer

Python is an easy language, so it's no surprise that it's good way to develop using GStreamer.

Some example scripts can be found in the [python_examples/](python_examples/) directory.

Other good GStreamer Python resources that I've found:

* [Getting started with GStreamer with Python](https://www.jonobacon.com/2006/08/28/getting-started-with-gstreamer-with-python/)
* [Python GStreamer Tutorial](http://brettviren.github.io/pygst-tutorial-org/pygst-tutorial.html)
* [Function reference](http://lazka.github.io/pgi-docs/#Gst-1.0)
* [Nice example script](https://github.com/rabits/rstream/blob/master/rstream.py)

### C/C++ with GStreamer

My favourite reference is [Valadoc](https://valadoc.org/gstreamer-1.0/index.htm)

# Problems or suggestions with this guide?

If you spot anything incorrect or incomplete, reports are welcome, either using [issues](issues) or [pull requests](pulls)
