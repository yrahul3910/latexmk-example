# Minimal example

This is a minimal example of how to set up LaTeX with `latexmk` and `watchman`. Set up `watchman` like so:

```sh
watchman watch .
watchman -- trigger . compile '*.tex' -- make pdf
```

You might want to change the `Makefile` to reflect the name of the main file.

Note: to install Latex-Mk, please use the included `latex-mk-2.1.tar.gz` file, which is a patched version of the official release with [this fix](https://sourceforge.net/p/latex-mk/bugs/27/) included. Once extracted, run

```sh
./configure
make
sudo make install
```
