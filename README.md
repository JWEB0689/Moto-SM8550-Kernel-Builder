# Moto SM8550 Kernel Builder

Automated GitHub Actions pipeline for building custom Android kernels for the Motorola SM8550 (5.15 GKI) platform.

## Features
- Fetches ZyC Clang toolchain
- Clones custom kernel source (defaults to LineageOS)
- Configurable Root Injection (KernelSU, SukiSU, etc.)
- SUSFS4KSU integration for root hiding
- KPM and BBR networking support

## Usage
Trigger the `Automated Kernel Builder` workflow under the Actions tab. You can configure:
- `KERNEL_SOURCE`: Git repository URL
- `KERNEL_BRANCH`: Branch to checkout
- `ROOT_METHOD`: Root injection strategy
- Toggle `ENABLE_SUSFS`, `ENABLE_BBR`, `ENABLE_KPM`

The compiled kernel image will be available as an artifact upon completion.