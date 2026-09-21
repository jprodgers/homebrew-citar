# homebrew-citar

A Homebrew tap for [CITAR](https://github.com/jprodgers/CITAR) — a Civilization V-style 4X game
for benchmarking language models.

```bash
brew install jprodgers/citar/citar
citar setup
```

`citar setup` looks for LM Studio, Ollama and other OpenAI-compatible servers already running on
your machine, and tells you what to install if it finds none. Then `citar` on its own starts
playing.

## Why a tap and not homebrew-core

homebrew-core requires every Python dependency to be listed as a pinned `resource` block — around
forty of them for CITAR, regenerated on every dependency change. Worth doing if CITAR is ever
submitted to core; not worth doing before anyone has asked for it.

## This repository is generated

`Formula/citar.rb` is copied from
[`packaging/homebrew/citar.rb`](https://github.com/jprodgers/CITAR/tree/main/packaging/homebrew)
in the CITAR repository, with the version and checksum filled in by `scripts/release_checksums.py`
at each release. Edit it there, not here.

Problems with the formula belong in
[CITAR's issue tracker](https://github.com/jprodgers/CITAR/issues).

## Licence

MPL-2.0, the same as CITAR. See [LICENSE](LICENSE).
