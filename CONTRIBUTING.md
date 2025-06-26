# Contributing to "Deliver value daily"

## Types of contributions

Contributions are welcome via the [GitHub PR mechanism](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork), subject to approval.

Particularly welcome are:

- Additions of techniques to help deliver value daily
- Changes that improve clarity, especially if they increase conciseness
- Changes that improve the accessibility of the site
- Technical changes that improve the performance of https://delivervaluedaily.dev/
- Fixing of typos

In most cases before raising a PR it's best to start a [GitHub issue](https://github.com/delivervaluedaily/manifesto/issues), or discussion in either [GitHub discussions](https://github.com/delivervaluedaily/manifesto/discussions) or the ["Deliver value daily" Discord server](https://discord.gg/Y5SvjeFnAF).

## Where to make contributions

- The bulk of the manifesto is in [README.md](./README.md) in Markdown format, with a small amount of HTML
- The header, footer, styles and other technical aspects of the site are in the Jinja2 template [index.jinja](./index.jinja)

## Long-form content

The site at https://delivervaluedaily.dev/ is deliberately short. Links to long-form content hosted elsewhere may be added in future.

If you have suggestions for links to long-form content, feel free to raise a [GitHub discurssion](https://github.com/delivervaluedaily/manifesto/discussions) or [Discord discussion](https://discord.gg/Y5SvjeFnAF).

## Building "Deliver value daily" locally

The site at https://delivervaluedaily.dev/ is designed so that only a single HTTPS request is required to fully display the page in browsers.

See [.github/workflows/deploy-to-github-pages.yml](./.github/workflows/deploy-to-github-pages.yml) for how the page is built in GitHub Actions. The page can be built locally by either:

- Copy and pasting individual lines into a terminal
- Using [act](https://github.com/nektos/act), for example by `act --container-architecture linux/amd64 --job build --bind`

The site is built into the `_site/` directory, and its `index.html` can be opened with a browser.

## Licensing of contributions

All submitted changes must be marked [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
