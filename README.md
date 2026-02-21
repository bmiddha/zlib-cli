# zlib-cli

A simple command-line tool for compressing and decompressing data using zlib.

## Usage

```sh
zcli deflate [file]    # compress data
zcli inflate [file]    # decompress data
```

If no file is provided, data is read from stdin.

## Examples

```sh
# Compress a file
zcli deflate input.txt > compressed.zlib

# Decompress a file
zcli inflate compressed.zlib > output.txt

# Pipe from stdin
echo "hello" | zcli deflate > compressed.zlib
```

## Requirements

- Python 3
