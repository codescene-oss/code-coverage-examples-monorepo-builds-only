# CodeScene Code Coverage examples - monorepo - builds only (no PRs)

This repository demonstrates how CodeScene supports code coverage gates in a CI build pipeline.

As such, this repository is part of the [CodeScene product documentation](https://codescene.io/docs/guides/code-coverage-gates/check-code-coverage-in-pull-and-merge-requests.html).

That [documentation](https://codescene.io/docs/guides/code-coverage-gates/check-code-coverage-in-pull-and-merge-requests.html) explains how to enable code coverage gates on your own repositories.

In [.github/workflows](./.github/workflows), you will find corresponding build pipelines definitions.

The reusable `check-coverage` action takes a numeric `project-id`, passes it to
`cs-coverage check --project-id`, and accepts an optional `onprem-url` for
CodeScene On-prem. For Cloud projects, the action uses the CLI's default API URL.

