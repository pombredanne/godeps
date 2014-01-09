# GoDeps

Simple dependency management for Go.
Some code borrowed from johnny_deps.

A simple shell script that installs the version of your go dependency packages stored in a `deps.txt` file and uses [Goven](https://github.com/kr/goven) to transfer them to a third party folder in your project named `third_party`.
It then renames your import paths in your go files for you (for only packages in deps.txt).


### Usage

1. Install [Goven](https://github.com/kr/goven).
2. Copy the `godeps` file to your Go project root. And `chmod +x godeps` if needed.
3. Create a deps.txt file in your project root `touch deps.txt`. See the example deps.txt included.
4. Run godeps `./godeps`


### What it does

It installs the version of the go package in the `deps.txt` file and uses goven
to copy it to a third party folder in your project named `third_party`.

*Works for git, hg and bzr packages.*
