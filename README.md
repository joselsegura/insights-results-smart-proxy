# insights-results-smart-proxy

[![GoDoc](https://godoc.org/github.com/RedHatInsights/insights-results-smart-proxy?status.svg)](https://godoc.org/github.com/RedHatInsights/insights-results-smart-proxy)
[![GitHub Pages](https://img.shields.io/badge/%20-GitHub%20Pages-informational)](https://redhatinsights.github.io/insights-results-smart-proxy/)
[![Go Report Card](https://goreportcard.com/badge/github.com/RedHatInsights/insights-results-smart-proxy)](https://goreportcard.com/report/github.com/RedHatInsights/insights-results-smart-proxy)
[![Build Status](https://ci.ext.devshift.net/buildStatus/icon?job=RedHatInsights-insights-results-smart-proxy-gh-build-master)](https://ci.ext.devshift.net/job/RedHatInsights-insights-results-smart-proxy-gh-build-master/)
![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/RedHatInsights/insights-results-smart-proxy)
[![License](https://img.shields.io/badge/license-Apache-blue)](https://github.com/RedHatInsights/insights-results-smart-proxy/blob/master/LICENSE)

Smart proxy for insights results

<!-- vim-markdown-toc GFM -->

* [Description](#description)
* [Documentation](#documentation)
* [Makefile targets](#makefile-targets)
* [Contribution](#contribution)
* [Package manifest](#package-manifest)

<!-- vim-markdown-toc -->

## Description

Insights Results Smart Proxy is a service that acts as a proxy between the different external
data pipeline clients and the different services providing the required information.

It provides access to the [Insights Results Aggregator](https://github.com/RedHatInsights/insights-results-aggregator)
and to the [Insights Content Service](https://github.com/RedHatInsights/insights-content-service),
providing the clients with different endpoints for accesing both report results and rule content metadata
from a single service.

## Documentation

Documentation is hosted on Github Pages <https://redhatinsights.github.io/insights-results-smart-proxy/>.
Sources are located in [docs](https://github.com/RedHatInsights/insights-results-smart-proxy/tree/master/docs).


## Makefile targets

```
Usage: make <OPTIONS> ... <TARGETS>

Available targets are:

clean                Run go clean
build                Build binary containing service executable
fmt                  Run go fmt -w for all sources
lint                 Run golint
vet                  Run go vet. Report likely mistakes in source code
cyclo                Run gocyclo
ineffassign          Run ineffassign checker
shellcheck           Run shellcheck
errcheck             Run errcheck
goconst              Run goconst checker
gosec                Run gosec checker
abcgo                Run ABC metrics checker
style                Run all the formatting related commands (fmt, vet, lint, cyclo) + check shell scripts
run                  Build the project and executes the binary
test                 Run the unit tests
help                 Show this help screen
```

## Contribution

Please look into document [CONTRIBUTING.md](CONTRIBUTING.md) that contains all information about how to
contribute to this project.

## Package manifest

Package manifest is available at [docs/manifest.txt](docs/manifest.txt).
