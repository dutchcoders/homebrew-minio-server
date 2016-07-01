homebrew-minio
===============
[![Build Status](https://travis-ci.org/dutchcoders/homebrew-minio.svg?branch=master)](https://travis-ci.org/dutchcoders/homebrew-minio)

Homebrew formula for minio.

## Usage

```bash
$ brew tap dutchcoders/homebrew-minio
$ brew install minio
```

## Troubleshooting

* Make sure you're using the right formula.  `brew info minio` should have a
  From line similar to this:

  ```text
  From: https://github.com/dutchcoders/homebrew-minio/blob/master/Formula/minio.rb
  ```

  If your formula points elsewhere, then you need to retap the minio formula.
  Do so with the following sequence of commands:

  ```text
  brew uninstall minio --force
  brew prune
  brew tap dutchcoders/homebrew-minio
  brew tap --repair
  brew install minio
  ```
* Run `brew update` — then try again.
* Run `brew doctor` — the doctor diagnoses common issues.
* You can create a gist log with `brew gist-logs minio`.
* Use `--verbose` to get the verbose output, i.e. `brew install --verbose minio`.
* Use `--debug` to be in the debug mode. In the debug mode, when failing, you
  can go into the interactive shell to check the building files before homebrew
  neutralizing them.
