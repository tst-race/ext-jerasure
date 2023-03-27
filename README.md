# Jerasure for RACE

This repo provides scripts to custom-build the
[Jerasure library](https://jerasure.org/) for RACE.

## License

The Jerasure library is licensed under the 3-Clause BSD license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

Jerasure has dependencies on the following custom-built libraries:

* GF-Complete

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build Jerasure.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-jerasure.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-jerasure
```

## Platforms

Jerasure is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`
* `android-x86_64`
* `android-arm64-v8a`

## How It Is Used

Jerasure is used by slothy.
