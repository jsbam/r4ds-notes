# r4ds-notes

See https://github.com/higgi13425/quarto-live-book/

## Known Issues

**Windows Path Resolution Error**: The webr/live extension had a module loading issue on Windows. Fixed by modifying `_extensions/r-wasm/live/live.lua` to use `quarto.utils.resolve_path()` instead of `require()` for loading `tinyyaml.lua`.
