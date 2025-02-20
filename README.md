# oItsMineZKernel for Exynos 9820/9825 Devices (S10/Note10)

<img src="https://github.com/rifsxd/KernelSU-Next/blob/next/assets/kernelsu_next.png" style="width: 96px;" alt="logo">

ExtremeKernel with KernelSU Next & SuSFS Based on [ExtremeKernel](https://github.com/Ocin4ever/ExtremeKernel) by [`Ocin4ever`](https://github.com/Ocin4ever) & [`ExtremeXT`](https://github.com/ExtremeXT)

## Features

- KernelSU Next
- SuSFS

## How to Install
Warning: `Please backup your modules before flashing this kernel, as all installed modules may be lost.`
- Flash Zip file via `TWRP`
- Install `KernelSU Next` from [Here](https://github.com/rifsxd/KernelSU-Next/releases)
- Install `susfs4ksu module` from [Here](https://github.com/sidex15/susfs4ksu-module/releases)

## Supported devices:

G970F - S10e - beyond0lte

G970N - S10e (Korean) - beyond0lteks

G973F - S10 - beyond1lte

G973N - S10 (Korean) - beyond1lteks

G975F - S10+ - beyond2lte

G975N - S10+ (Korean) - beyond2lteks

G977B - S10 5G - beyondx

G977N - S10 5G (Korean) - beyondxks

N970F - Note 10 - d1

N971N - Note 10 5G (Korean) - d1xks

N975F - Note 10+ - d2s

N976B - Note 10+ 5G - d2x

N976N - Note 10+ 5G (Korean) - d2xks

## Build instructions:

1. Set up build environment as per Google documentation

   <a href="https://source.android.com/docs/setup/start/requirements" target="_blank">https://source.android.com/docs/setup/start/requirements</a>

2. Properly clone repository with submodules (KernelSU and toolchains)

```html
git clone --recurse-submodules https://github.com/oItsMineZKernel/android_kernel_samsung_oneui6_exynos9820
```

3. Build for your device

```html
./build.sh -m d2s -k y
```

4. Fetch the flashable zip of the kernel that was just compiled

```html
build/out/[your_device]/oItsMineZKernel-OneUI6...zip
```

5. Flash it using a supported recovery like TWRP

6. Enjoy!

## Credits

- [`rifsxd`](https://github.com/rifsxd) for [KernelSU Next](https://github.com/rifsxd/KernelSU-Next)
- [`simonpunk`](https://gitlab.com/simonpunk) for [susfs4ksu (Kernel 4.14 Non-GKI)](https://gitlab.com/simonpunk/susfs4ksu/-/tree/kernel-4.14)
- [`Ocin4ever`](https://github.com/Ocin4ever) & [`ExtremeXT`](https://github.com/ExtremeXT) for [ExtremeKernel](https://github.com/Ocin4ever/ExtremeKernel)
