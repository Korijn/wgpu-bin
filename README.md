[![Build Status](https://korijn.visualstudio.com/wgpu-bin/_apis/build/status/Korijn.wgpu-bin?branchName=master)](https://korijn.visualstudio.com/wgpu-bin/_build/latest?definitionId=2&branchName=master)

# wgpu-bin

Optimized binaries for [wgpu-native](https://github.com/gfx-rs/wgpu) for use in Python projects.

That means each release includes binaries for the following platforms:

* MacOS 64-bit
* Windows 32-bit
* Windows 64-bit
* [Manylinux2010](https://www.python.org/dev/peps/pep-0571/) 32-bit
* [Manylinux2010](https://www.python.org/dev/peps/pep-0571/) 64-bit

Note: [manylinux1](https://www.python.org/dev/peps/pep-0513/) is not supported because wgpu requires a minimum version of X11 that is not available on the [PyPA docker images](https://github.com/pypa/manylinux).
