# markdown-render-speed-02

A fast drop-in replacement for marked 18.1.3 — make.fun competition entry.

`parse.js` exports `parse(markdown)`, returning exactly the HTML marked 18.1.3
renders with its default options (GFM on), dependency-free. `main.ts` is the
driver the harness runs: it reads every case from `/input/cases.json`, renders
each with `parse`, and writes `/output/html.json`.
