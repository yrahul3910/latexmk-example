# Minimal example

This is a minimal example of how to set up LaTeX with `latexmk` and `watchman`. Set up `watchman` like so:

```sh
watchman watch .
watchman -- trigger . compile '*.tex' -- make pdf
```

You might want to change the `Makefile` to reflect the name of the main file.
