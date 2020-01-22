[![Build Status](https://korijn.visualstudio.com/wgpu-bin/_apis/build/status/Korijn.wgpu-bin?branchName=master)](https://korijn.visualstudio.com/wgpu-bin/_build/latest?definitionId=2&branchName=master)

# wgpu-bin

Optimized binaries for [wgpu-native](https://github.com/gfx-rs/wgpu) for use in Python projects.

That means each release includes binaries for the following platforms:

* MacOS 64-bit
* Windows 32-bit
* Windows 64-bit
* [Manylinux1](https://www.python.org/dev/peps/pep-0513/) 32-bit
* [Manylinux1](https://www.python.org/dev/peps/pep-0513/) 64-bit

Note: Although the linux binaries are built on the [PyPA Manylinux2010 docker image](https://github.com/pypa/manylinux), they are also compatible with the [Manylinux1](https://www.python.org/dev/peps/pep-0513/) standard, and pass [auditwheel](https://github.com/pypa/auditwheel)'s checks! The reason we build on the Manylinux2010 docker image is that wgpu relies on a Rust package that requires a minimum version of X11 that is not available on the version of CentOS that the Manylinux1 docker image is based on.
