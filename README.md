# Yuri Clang

This is a [LLVM](https://llvm.org/) and [Clang](https://clang.llvm.org/) compiler toolchain built for kernel development. Builds are always made from the latest LLVM sources rather than stable releases, so complete stability cannot be guaranteed. 

This toolchain targets the AArch32, AArch64, and x86 architectures. It is built with ThinLTO to reduce compile times as much as possible. [Polly](https://polly.llvm.org/), LLVM's polyhedral loop optimizer, is also included for users who want to experiment with additional optimization. Note that this toolchain is **not** suitable for anything other than bare-metal development; it has not been built with support for any libc or userspace development in mind.

This is a Random build for my GKI kernel. The build scripts (powered by [tc-build](https://github.com/ClangBuiltLinux/tc-build)) & modified from [Neutron-Toolchains](https://github.com/Neutron-Toolchains/llvm-tc-build)