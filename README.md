# My R4DS notes using WebR

Interactive study notes for [R for Data Science (2nd Edition)](https://r4ds.hadley.nz/) by Hadley Wickham, Mine Çetinkaya-Rundel, and Garrett Grolemund.

**📖 Live Book:** <https://jsbam.github.io/r4ds-notes/>

## Overview

This Quarto book uses `WebR` and the `live-html` format to create an interactive learning environment where you can run R code directly in your browser—no local R installation required.

## Setup Guide

To create a similar Quarto book with WebR and live-html format, see an excellent guide at <https://github.com/higgi13425/quarto-live-book/>.

## Project Structure

This project is edited and built incrementally while reading R4DS book.

## Known Issues

### Windows Path Resolution Error

**Issue:** The webr/live extension had a module loading error on Windows due to path resolution.

**Solution:** Modified `_extensions/r-wasm/live/live.lua` to use `quarto.utils.resolve_path()` instead of `require()` for loading `tinyyaml.lua`.

## Resources

- [R for Data Science (2e)](https://r4ds.hadley.nz/): Original book
- [Quarto Books](https://quarto.org/docs/books): Quarto book project
- [WebR Documentation](https://docs.r-wasm.org/webr/latest/): `WebR` reference
- [Quarto Live Extension](https://github.com/r-wasm/quarto-live): `quarto-live` extension to embed interactive R code.

## License

These notes are for educational purposes. The original R4DS book is available under a Creative Commons license.