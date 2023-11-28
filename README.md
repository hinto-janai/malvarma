<div align="center">

<img src="src/img/banner_1920_640.png" width="100%"/>

[Cold wallet](https://en.wikipedia.org/wiki/Cryptocurrency_wallet#Cold_storage) guide for [Monero](https://getmonero.org)

![CI](https://github.com/hinto-janai/malvarma/actions/workflows/ci.yml/badge.svg)

</div>

## Contributing
The text sources are regular markdown files located in [`src/`](src).

This get compiled into HTML/JS/CSS with [`mdbook`](https://github.com/rust-lang/mdBook) into [`docs/`](docs), which are the files directly served by https://malvarma.org.

To build & test, install [`mdbook`](https://rust-lang.github.io/mdBook) and run:
```bash
mdbook build
```
at the repo root.

The files should be placed in `docs/` with an `index.html`.

Do not submit PRs with a pre-built `docs/` folder, only make changes to `src/`.

This guide should mostly be a list of instructions on setting up a cold wallet with sane defaults.

Detailed commentary, terminology, and tradeoffs are withheld on purpose - this guide should be as simple/practical as possible.
