# GoDeps

Simple dependency management for Go.

[![baby-gopher](https://raw2.github.com/drnic/babygopher-site/gh-pages/images/babygopher-badge.png)](http://www.babygopher.org)

### What it does

It installs the version of the go package in the `deps.txt` file and uses goven
to copy it to a third party folder in your project named `third_party`.

*Works for git, hg and bzr packages.*

### Usage

1. Install [Goven](https://github.com/kr/goven).
2. Copy the `godeps` file to your PATH. `chmod +x godeps` if needed.
3. Create a deps.txt file in your project root `touch deps.txt`. See the example deps.txt included.
4. Run `godeps`
