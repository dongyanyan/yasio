<p align="center"><a href="https://yasio.org" target="_blank" rel="noopener noreferrer"><img width="160" src="https://yasio.org/images/logo.png" alt="yasio logo"></a></p>

# *YASIO* - *Y*et *A*nother asynchronous *S*ocket *I*/*O*.
[![Build Status](https://travis-ci.com/yasio/yasio.svg?branch=master)](https://travis-ci.com/yasio/yasio)
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/d6qjfygtw2ewt9pf/branch/master?svg=true)](https://ci.appveyor.com/project/halx99/yasio)
[![Release](https://img.shields.io/badge/dev-v3.33.0-blue.svg)](https://github.com/yasio/yasio/releases)
[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/yasio/yasio/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/yasio/yasio.svg?label=Stars)](https://github.com/yasio/yasio)
[![GitHub forks](https://img.shields.io/github/forks/yasio/yasio.svg?label=Fork)](https://github.com/yasio/yasio)
[![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/yasio/yasio.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/yasio/yasio/context:cpp)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/yasio/yasio.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/yasio/yasio/alerts/)
[![Last Commit](https://badgen.net/github/last-commit/yasio/yasio)](https://github.com/yasio/yasio)

  
[![Supported Platforms](https://img.shields.io/badge/platform-ios%20%7C%20osx%20%7C%20android%20%7C%20win32%20%7C%20linux-green.svg?style=flat-square)](https://github.com/yasio/yasio)
[![Powered](https://img.shields.io/badge/Powered%20by-c4games-blue.svg)](http://c4games.com)  
  
**[简体中文](README.md)**
  
**yasio** is a multi-platform support and lightweight library with focus on asynchronous socket I/O for any client application, support windows & linux & apple & android & win10-universal.  

## Showcase
* [RAOL Mobile Game Project](https://hongjing.qq.com/): Since the game is published on Tencent Games at 2018.10.17, it's run at millions of devices.
* [x-studio IDE Project](https://en.x-studio.net/): The local LAN upgrade system is based on yasio.
* [xlua](https://github.com/c4games/xlua): Integrate yasio to xlua, make the unity3d game project based on xlua can use yasio lua bindings APIs.

## Docomentation
* Simplified Chinese: [https://docs.yasio.org/](https://docs.yasio.org/)
* English: [https://docs.yasio.org/en/latest/](https://docs.yasio.org/en/latest/)

## Simple run tcptest with g++
```sh
g++ tests/tcp/main.cpp --std=c++11 -DYASIO_HEADER_ONLY -lpthread -I./ -o tcptest && ./tcptest
```

## Build more examples with cmake
```sh
git clone https://github.com/yasio/yasio
cd yasio
git submodule update --init --recursive
cd build
cmake ..

# Use cmake command to build examples & tests, 
# or open yasio.sln with visual studio(2013~2019 supported) at win32 platform
cmake --build . --config Debug
```

## Features: 
* support IPv6-only network.  
* support multi-connections at one thread.  
* support deadline timer.  
* support unpack tcp packet internal, user do not need to care it.  
* support lua bindings  
* support cocos2d-x jsb  
* support CocosCreator jsb2.0  
* support Unity3D
* support multicast
* support ssl client with openssl
* support async resolve with c-ares
* Support header only with YASIO_HEAD_ONLY=1 set at config.hpp or compiler flags
  
## Core framework
![image](https://yasio.org/images/framework_en.png)  

## For more detail usage: see [wiki](https://github.com/yasio/yasio/wiki)

