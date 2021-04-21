# signadot-install-testing

[![Install Signadot](https://github.com/abatilo/signadot-install-testing/actions/workflows/install-signadot.yml/badge.svg)](https://github.com/abatilo/signadot-install-testing/actions/workflows/install-signadot.yml)

There's a bug in signadot that does not handle an API change that seems to have
been introduced in Kubernetes 1.19+.

To help verify that there's been a fix made, I've created this repository which
uses GitHub Actions to run an integration test across multiple versions of
Kubernetes.

We use `kind` to run a Kubernetes cluster in the GitHub Action, and then use
the installation instructions for signadot found
[here](https://docs.signadot.com/installation/installation/cluster-component/signadot-sidecars).

Look at [the Actions tab](https://github.com/abatilo/signadot-install-testing/actions) to view more results and logs.
