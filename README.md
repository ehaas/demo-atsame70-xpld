## Build Instructions
This repository has one submodule (Unity unit testing framework) so when cloning make sure to include the `--recurse-submodules` flag.  
If the repo has already been cloned and the `--recurse-submodules` flag was not included you can run `git submodule update --init --recursive`  


```
mkdir -p _build
cd _build
cmake .. -G Ninja -DCMAKE_TOOLCHAIN_FILE=../cmake/arm-gcc-toolchain.cmake
cmake --build .
```
