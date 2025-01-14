# clang-tools static binaries

[![Build](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/build-amd64.yml/badge.svg)](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/build-amd64.yml)
[![Test](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/test.yml/badge.svg)](https://github.com/cpp-linter/clang-tools-static-binaries/actions/workflows/test.yml)
![](https://img.shields.io/badge/platform-linux--64%20%7C%20win--64%20%7C%20osx--64%20-blue)

Includes clang-format, clang-tidy, clang-query and clang-apply-replacements. 

The supported versions are as follows:

|OS/Version |19|18 |17 |16 |15 |14 |13 |12 |11 |10 |9  |8  |7  |
|-----------|--|---|---|---|---|---|---|---|---|---|---|---|---|
|Linux 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |    
|Window 64  |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |
|macOS 64   |✔️|✔️ |✔️|✔️|✔️ |✔️|✔️ |✔️ |✔️|✔️| ✔️|✔️|✔️ |

> [!CAUTION]
> clang-tidy v18+ not working or unavailable.
> * clang-tidy-18_macosx-amd64 - Reason: tried: '/usr/lib/libz.1.dylib' (no such file)
> * clang-tidy-19_macosx-amd64 - File size exceeds 2GB, unable to upload to GitHub releases.

## Download

Grab clang-tools static binaries for your platform from [Releases](https://github.com/cpp-linter/clang-tools-static-binaries/releases) tab!

## Motivation behind this repo

I used to contribute to different repositories and they often use different versions of clang-format.

I could either compile clang-format for each one I want to have or I could try messing up with my package system (I use Arch Linux btw) and try installing all of them on my system.
This can very quickly get out of hand, hence I created this repository.

These binaries aim to:
- be as small as possible
- not require any additional dependencies apart from OS itself

This repository ([cpp-linter/clang-tools-static-binaries](https://github.com/cpp-linter/clang-tools-static-binaries)) is forked from [muttleyxd/clang-tools-static-binaries](https://github.com/muttleyxd/clang-tools-static-binaries).

## How can I trust this repository?

- Verify sha512sums of binaries against output from GitHub Actions to make sure binaries are not modified
- Fork this repository and run GitHub actions on your behalf
- Build manually using steps using commands from [.github/workflows](https://github.com/cpp-linter/clang-tools-static-binaries/tree/master/.github/workflows)

## More clang-tools

If there's any interest I could add more tools, or a build for new OS (ex. FreeBSD)
