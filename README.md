# veya-lang.org

The website of the [Veya](https://veya-lang.org) language, served by GitHub Pages.

- `index.src.html` and `guide.src.html` are the templates; `samples/*.veya` are the
  homepage's code (each one compiles: `veya check samples/*.veya`).
- `tools/build.py` makes `index.html`, `guide.html` (from sections of the
  compiler's README) and `code.css`:

```sh
python3 -m venv .venv && .venv/bin/pip install markdown pygments
.venv/bin/python tools/build.py ../veya/README.md
```
