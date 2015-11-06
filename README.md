# y4m [![Build Status](https://travis-ci.org/PistonDevelopers/y4m.png?branch=master)](https://travis-ci.org/PistonDevelopers/y4m) [![crates.io](https://img.shields.io/crates/v/y4m.svg)](https://crates.io/crates/y4m)

YUV4MPEG2 (.y4m) Reader/Writer. [Format specification](http://wiki.multimedia.cx/index.php?title=YUV4MPEG2).

## Usage

```rust
extern crate y4m;
```

See [API documentation](http://docs.piston.rs/resize/resize/) for overview of all available methods. See also [this example](examples/resize.rs) on how to resize input y4m into grayscale y4m of different resolution:

```bash
ffmpeg -i in.mkv -f yuv4mpegpipe - | target/debug/examples/resize - 640x360 - | mpv -
```

## License

Library is licensed under [MIT](LICENSE).
