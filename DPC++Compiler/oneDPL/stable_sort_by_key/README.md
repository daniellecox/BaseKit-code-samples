# Stable sort by key sample

This example demonstrates how to use `counting_iterator` and `zip_iterator`.

The example fills two buffers and then sorts them both using `zip_iterator`.
It models stable sort by key: during the sorting of 2 sequences (keys and values) only keys are compared but both keys and values are swapped.

The computations are performed using Intel® oneAPI DPC++ library (oneDPL).

| Optimized for                   | Description                                                                        |
|---------------------------------|------------------------------------------------------------------------------------|
| OS                              | Linux Ubuntu 18.04                                                                 |
| Hardware                        | Skylake with GEN9 or newer                                                         |
| Software                        | Intel® oneAPI DPC++ Compiler (beta)                                                |
| What you will learn             | How to use `counting_iterator` and `zip_iterator` that are a part of DPC++ Library |
| Time to complete                | At most 5 minutes                                                                  |

## License

This code sample is licensed under MIT license.

## How to build

```bash
# To this point you should have
# - Data Parallel C++ Library installed and
# - environment variables set up to use it

mkdir build && cd build  # execute in this directory

```

### Linux

```bash
CXX=dpcpp cmake ..
cmake --build .  # or "make"
cmake --build . --target run  # or "make run"
```

### Windows

```bash
cmake -G "MinGW Makefiles" -DCMAKE_MAKE_PROGRAM=gmake -DCMAKE_CXX_COMPILER=dpcpp-cl ..
cmake --build .  # or "gmake"
cmake --build . --target run  # or "gmake run"
```
