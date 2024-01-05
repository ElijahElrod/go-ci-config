# Github config and workflows

In this folder there is configuration for codecoverage, dependabot, and ci
workflows (gofmt, golangci, and running tests).

This folder can be or was merged using a --allow-unrelated-histories merge
strategy from <https://github.com/ElijahElrod/go-ci-config.git/> which provides a CI base for Go projects. 
By using this strategy, the history of the CI repo is included in your repo, and future updates to
the CI can be merged later.

To perform this merge run:

```shell
git remote add ci https://github.com/ElijahElrod/go-ci-config.git
git fetch ci
git merge --allow-unrelated-histories ci/main
```

Workflows for Go inspired by this Rust Variant -> https://github.com/jonhoo/rust-ci-conf