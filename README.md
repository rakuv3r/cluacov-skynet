<div align="center">
    <h1>cluacov-skynet</h1>
    <p>C performance extension for LuaCov in Skynet framework</p>
</div>

[中文](docs/README-zh.md)

## What is it

A fork of [mpeterv/cluacov](https://github.com/mpeterv/cluacov) with Skynet optimizations. Provides faster code coverage tracking than pure Lua implementation.

## Installation

```bash
git clone https://github.com/rakuv3r/cluacov-skynet.git
cd cluacov-skynet
gcc -shared -fPIC -o hook.so src/cluacov/hook.c
```

Replace your existing cluacov hook:
```bash
# Find where cluacov is installed
luarocks show cluacov

# Replace with Skynet version
cp hook.so /path/to/cluacov/hook.so
```

## Usage

Works automatically with [luacov-skynet](https://github.com/rakuv3r/luacov-skynet).

## License

[MIT License](LICENSE)