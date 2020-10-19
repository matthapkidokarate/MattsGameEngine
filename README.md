# Matt's Game Engine

A game engine made in C (maybe with some additional C++) to work on imperative programming.
This engine is designed to take advantage of OpenGL available in modern graphical hardware.

## Building
This project is built using CMake. The actual engine is a shared library
which is built as a dependency of all examples. To build just the SO or DLL,
run cmake and build the target `Matts_Game_Engine_Engine`.
### Required packages
On a base ubuntu install, `libx11-dev libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev libgl-dev libglu-dev`
are required.
## Using
##### TODO: Make a WIKI with information on using the engine.
To use the engine, add this to your `CMakeLists.txt`. The CMakeLists.txt used here is the one in this folder.
```
add_subdirectory(path/to/CMakeLists.txt)
target_link_libraries(YOUR_TARGET_NAME Matts_Game_Engine_Engine)
```
###### Core.h
Core.h must be included in every file that utilizes the engine. It must be included below RequiredGlobals. in your main.
###### RequiredGlobals.h
For the file that contains your entry point, please include `#include <Matts-Engine/RequiredGlobals.h>`. This contains the
required globals that must only be included in one translation unit.

## License
Matt's Game Engine is licensed under a `BSD 3-Clause License`. 
This license is as follows:
```
Matt's Game Engine is licensed under a BSD 3-Clause License

BSD 3-Clause License

Copyright (c) 2020, Matthew Krueger
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Thanks
Thanks to [The Cherno](https://www.youtube.com/channel/UCQ-W1KE9EYfdxhL6S4twUNw)
for the game engine series. 