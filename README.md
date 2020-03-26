# ffmpeg-decoder

Decodes input audio files and converts sample format to signed 16bit little endian.


## Rodio Source

`Decoder` implies rodio's `Source` trait, as well as `Iterator`. Enable feature 
flag `rodio_source` to include this. Decoder can then be used as a source for Rodio,
with the benefits of being able to decode everything ffmpeg supports.


## CLI


### Convert input file to signed 16bit and save as `.raw` alongisde original
```
cargo run --release -- convert path/to/test.mp3
```

### Play with rodio
```
cargo run --release -- play path/to/test.flac
```