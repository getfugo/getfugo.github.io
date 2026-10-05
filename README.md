# getfugo.github.io

This repository publishes https://getfugo.github.io/, the documentation of
[fugo](https://github.com/getfugo/fugo). Its only content is the workflow that does so,
`.github/workflows/publish.yml`. Once a day, and when run by hand, the workflow:

1. builds `docs/` of getfugo/fugo at the latest release, with that release's binary;
2. adds the benchmark history that fugo's CI keeps on its `gh-pages` branch, for the
   [Benchmarks](https://getfugo.github.io/about/benchmarks/) page;
3. deploys the site with GitHub Pages (Settings → Pages → Source: GitHub Actions).

To change the documentation, edit `docs/` in getfugo/fugo. `DEVELOPMENT.md` there, under
"Benchmarks", describes the measurements.

The site this repository held until 2025-10-13, the Go version's documentation (v0.148.2), is
the tag `go-docs-v0.148.2`.
