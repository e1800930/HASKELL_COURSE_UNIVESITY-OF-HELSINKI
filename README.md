# Haskell MOOC

<p align="center"><img alt="Course logo" src="img/haskell-mooc-logo.svg" width="400" align="center"></p>

University of Helsinki
This is the solution to the course 
This only for self-documentation and studying purpose
Feel free to come up with any better solutions or contribute to this work.
## About the course

This is an online course on Functional Programming that uses the
Haskell programming language. You can study at your own pace. All the
material and exercises are openly available.

The course is intended to be followed through the [Course
page](https://haskell.mooc.fi), but in case the course page is down or
you want an offline backup, the course material is also available in
this repository ([part1.html](part1.html), [part2.html](part2.html)).

## What is Haskell?
Haskell is a general-purpose, statically-typed, purely functional programming language with type inference and lazy evaluation.

To run Haskell programs, please visit this page for extra guidance on installation:
[Haskell Installation page](https://www.haskell.org/ghcup/install/)

<b>Note! GHC 8.10.7 has a GHCi bug that makes editing lines impossible on ARM-based systems. As a workaround, use TERM=dumb stack ghci. More info here.</b>

To uninstall Haskell:
On Linux OS:
Use CMD
Step 1:
```
ghcup nuke
```
Step 2: then make sure any ghcup added lines in your ~/.bashrc (or similar) are removed.


On Windows:
On windows, right click on the Uninstall Haskell.ps1 PowerShell script on your Desktop and select Run with PowerShell.


## Exercises

Exercises can be found under `exercises/` directory. All required dependencies
can be downloaded and built with:

```
stack build
```

Exercises are Haskell source code files named `Set1.hs`, `Set2.hs` and so on.
You complete the exercises by editing the file according to the instructions in
the file. You can check your answers by running

```
stack runhaskell SetXTest.hs
```

in the `exercises/` directory. Remember to replace `X` with the number
of the set you are working on.

See [the material](part1.html#working-on-the-exercises) for more info.

## Troubleshooting

Here are some fixes for common problems with `stack build`:

- If you get an error like `While building package zlib-0.6.2.3`, you need to install the zlib library headers. The right command for Ubuntu is `sudo apt install zlib1g-dev`.
- If you get an error like `Downloading lts-18.18 build plan ... RedownloadInvalidResponse`, your version of stack is too old. Run `stack upgrade` to get a newer one.

## Reporting errors

If you notice an error in these materials, you can report it via
- an issue or pull request in this repository (see [CONTRIBUTING.md](CONTRIBUTING.md))
- the course [channel on Telegram](https://t.me/haskell_mooc_fi)
