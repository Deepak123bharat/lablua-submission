# GSoC 2021 Final Submission
### Quick links of the contribution.

* [Rocks-fs](https://github.com/Deepak123bharat/rocks-fs) stand-alone module for the filesystem. [link](https://github.com/Deepak123bharat/rocks-fs/commits/master)
* [Rocks-dir](https://github.com/Deepak123bharat/rocks-dir) stand-alone module to handling pathnames. [link](https://github.com/Deepak123bharat/rocks-dir/commits/master)
* [Rocks-fun](https://github.com/Deepak123bharat/rocks-fun) stand-alone module basic functional utilities. [link](https://github.com/Deepak123bharat/rocks-fun/commits/master)
* [Rocks-patch](https://github.com/Deepak123bharat/rocks-patch) stand-alone module for patch utility to apply unified diffs. [link](https://github.com/Deepak123bharat/rocks-patch/commits/master)
* [Rocks-tar](https://github.com/Deepak123bharat/rocks-tar) A pure-Lua implementation of untar. [link](https://github.com/Deepak123bharat/rocks-tar/commits/master)
* [Rocks-zip](https://github.com/Deepak123bharat/rocks-zip) A Lua implementation of .zip and .gz file. [link](https://github.com/Deepak123bharat/rocks-zip/commits/master)
* [Rocks-sysdetect](https://github.com/Deepak123bharat/rocks-sysdetect) stand-alone module for detecting operating system. [link](https://github.com/Deepak123bharat/rocks-sysdetect/commits/master)
* [Luarocks-unit](https://github.com/Deepak123bharat/luarocks/tree/luarocks-unit) Luarocks branch which uses all the above stand-alone modules. [link](https://github.com/Deepak123bharat/luarocks/commits/luarocks-unit)

## Table of Contents

* [Overview](#Overview)
* [Installing modules using Luarocks](#installing-modules-using-luarocks)
* [Usage](#Usage)
* [Work Status](#work-status)
    * [What is done](#what-is-done)
    * [TODO](#todo)
    
## Overview

This project aims to split the Luarocks project into more manageable chunks, making parts of it into libraries and providing a typed API for LuaRocks modules, specified using Teal, a typed dialect of Lua. 

<img border="0" src="https://github.com/Deepak123bharat/lablua-submission/blob/main/pic1.png">

 ## Installing modules using Luarocks. 
 
 ```
 luarocks install rocks-fs
 luarocks install rocks-fun
 luarocks install rocks-dir
 luarocks install rocks-patch
 luarocks install rocks-tar
 luarocks install rocks-zip
 luarocks install rocks-sysdetect
 ```
 
 ## Usage
 
 ```lua
 local fs = require("rocks.fs")
 local fun = require("rocks.fun")
 local dir = require("rocks.dir")
 local patch = require("rocks.patch")
 local tar = require("rocks.tar")
 local zip = require("rocks.zip")
 local sysdetect = require("rocks.sysdetect")
 ```
 
## Work Status

### What is done
 
 * [Luarocks-unit](https://github.com/Deepak123bharat/luarocks/tree/luarocks-unit) branch that uses all the stand-alone modules
 * Stand-alone modules 
    * [rocks-fs](https://github.com/Deepak123bharat/rocks-fs)
    * [procks-fun](https://github.com/Deepak123bharat/rocks-fun)
    * [rocks-dir](https://github.com/Deepak123bharat/rocks-dir)
    * [rocks-patch](https://github.com/Deepak123bharat/rocks-patch)
    * [rocks-tar](https://github.com/Deepak123bharat/rocks-tar)
    * [rocks-zip](https://github.com/Deepak123bharat/rocks-zip)
    * [rocks-sysdetect](https://github.com/Deepak123bharat/rocks-sysdetect)
 * Unit Testing With Busted for all the stand alone modules and luarocks-unit branch
 * Type definitions for the libraries
 * Continuous Integration using [AppVeyor](https://www.appveyor.com/) and [Travis](https://travis-ci.com/) for all the modules and luarocks-unit 

      Stand-alone Modules | Travis | AppVeyor
      --- | --- | --- 
      rocks-fs | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-fs.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-fs) | [![Build status](https://ci.appveyor.com/api/projects/status/lc19rwfe8g4n0rri/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-fs/branch/master)
      rocks-fun | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-fun.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-fun) | [![Build status](https://ci.appveyor.com/api/projects/status/ecab3c0orikoj9xr/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-fun/branch/master)
      rocks-dir | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-dir.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-dir) | [![Build status](https://ci.appveyor.com/api/projects/status/wsfxtp5x6k4a5e22/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-dir/branch/master)
      rocks-patch | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-patch.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-patch) | [![Build status](https://ci.appveyor.com/api/projects/status/mk3tddiub5vltlb1/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-patch/branch/master)
      rocks-tar | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-tar.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-tar) | [![Build status](https://ci.appveyor.com/api/projects/status/csaklrit7kg06kvw/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-tar/branch/master)
      rocks-zip | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-zip.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-zip) | [![Build status](https://ci.appveyor.com/api/projects/status/tqs3mohxqgv6xspg/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-zip/branch/master)
      rocks-sysdetect | [![Build Status](https://travis-ci.com/Deepak123bharat/rocks-sysdetect.svg?branch=master)](https://travis-ci.com/github/Deepak123bharat/rocks-sysdetect) | [![Build status](https://ci.appveyor.com/api/projects/status/67phoc7a7rtsh73b/branch/master?svg=true)](https://ci.appveyor.com/project/Deepak123bharat/rocks-sysdetect/branch/master)
### TODO
 
 * Providing typed API for all the modules
