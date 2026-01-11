# About this project

This quarto book project is published at <https://jsbam.github.io/r4ds-notes/>.

In this project, I use webr and quarto live to document my notes of the book **R for Data Science (2ed)**. To set up a quarto book project using live-html format and webr, useful instructions may be found at <https://github.com/higgi13425/quarto-live-book/>.

## Known Issues

**Windows Path Resolution Error**: The webr/live extension had a module loading issue on Windows. Fixed by modifying `_extensions/r-wasm/live/live.lua` to use `quarto.utils.resolve_path()` instead of `require()` for loading `tinyyaml.lua`.
