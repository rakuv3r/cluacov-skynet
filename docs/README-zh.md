<div align="center">
    <h1>cluacov-skynet</h1>
    <p>Skynet 框架的 LuaCov C 性能扩展</p>
</div>

[English](../README.md)

## 项目简介

基于 [mpeterv/cluacov](https://github.com/mpeterv/cluacov) 改进，专为 Skynet 框架优化的 C 语言扩展。提供比纯 Lua 实现更快的代码覆盖率追踪性能。

## 安装方法

```bash
git clone https://github.com/rakuv3r/cluacov-skynet.git
cd cluacov-skynet
gcc -shared -fPIC -o hook.so src/cluacov/hook.c
```

替换现有的 cluacov hook：
```bash
# 找到 cluacov 安装位置
luarocks show cluacov

# 用 Skynet 版本替换
cp hook.so /path/to/cluacov/hook.so
```

## 使用方法

与 [luacov-skynet](https://github.com/rakuv3r/luacov-skynet) 配合自动工作。

## 开源协议

[MIT License](../LICENSE)