# Installing TensorFlow on Orange Pi PC PLUS (and probably any H3 based SBC)

* [Building from source (hard)](#building-from-source)
* [Credits](#credits)
* [License](#license)


## Building from Source

[_Step-by-step guide_](GUIDE.md)

If you aren't able to make the wheel file from the previous section work, you may need to build from source. Additionally, if you want to use features that have not been included in an official release, such as the [initial distributed runtime](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/core/distributed_runtime), you'll have to build from source. 

See the [step-by-step guide here](GUIDE.md). **Warning: it takes a while.**

## Credits

While the final pieces of grunt work were done primarily by myself and @petewarden, this effort has been going on for almost as long as TensorFlow has been open-source, and involves work that spans multiple months in separate codebases. This is an incomprehensive list of people and their work I ran across while working on this.

The majority of the source-building guide is a modified version of [these instructions for compiling TensorFlow on a Jetson TK1](http://cudamusing.blogspot.com/2015/11/building-tensorflow-for-jetson-tk1.html). Massimiliano, you are the real MVP. _Note: the TK1 guide was [updated on June 17, 2016](http://cudamusing.blogspot.com/2016/06/tensorflow-08-on-jetson-tk1.html)_

@vmayoral put a huge amount of time and effort trying to put together the pieces to build TensorFlow, and was the first to get something close to a working binary.

A bunch of awesome Googlers working in both the TensorFlow and Bazel repositories helped make this possible. In no particular order: @vrv, @damienmg, @petewarden, @danbri, @ulfjack, @girving, and @nlothian

_Issue threads of interest:_

* [Initial issue for building Bazel on ARMv7l](https://github.com/bazelbuild/bazel/issues/606)
* [First thread about running TensorFlow on RPi](https://github.com/tensorflow/tensorflow/issues/254)
* [Parallel thread on building TensorFlow on ARMv7l](https://github.com/tensorflow/tensorflow/issues/445)
	* This is where the most recent conversation is located

## License

Subdirectories contained within the `third_party` directory each contain relevant licenses for the code and software within those subdirectories.

The file TENSORFLOW_LICENSE applies to the binaries distributed in the [releases.](https://github.com/samjabrahams/tensorflow-on-raspberry-pi/releases)

The file LICENSE applies to other files in this repository. I want to stress that a majority of the lines of code found in the guide of this repository was created by others. If any of those original authors want more prominent attribution, please contact me and we can figure out how to make it acceptable.

---

_[Back to top](#installing-tensorflow-on-orange-pi-pc-plus-and-probably-any-h3-based-sbc)_
