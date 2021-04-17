# Scala Test Template

## Overview

This is a variant of the sbt getting-started tutorial [here](https://www.scala-sbt.org/1.x/docs/sbt-by-example.html).

The purpose of this repo is to provide a minimum fileset required to get an sbt/metals project up-and-running, while still providing some basic functionality to demonstrate the scala workflow.

## Reference

* [SBT Native Packager commands](https://www.scala-sbt.org/sbt-native-packager/gettingstarted.html)
  * Docker commands, etc.

## Setup

### Environment

* (WSL) Ubuntu 20.04.2 LTS

### Tooling

* [VS Code](https://code.visualstudio.com/)
* [SBT (v1.5.0)](https://www.scala-sbt.org/download.html)
* OpenJDK version "1.8.0_282"

### VS Code Extensions

* [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
* [Scala Syntax (official)](https://marketplace.visualstudio.com/items?itemName=scala-lang.scala)
* [Scala (Metals)](https://marketplace.visualstudio.com/items?itemName=scalameta.metals)
* [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) (Optional)

## Quick Reference

*Note: `sbt:_>` refers to a command being executed in the sbt terminal.*

| Description | Command |
|-------------|---------|
| Start the sbt shell | `sbt` |
| Exit the sbt shell | `sbt:_> exit` |
| Build & Run | `sbt:_> run` |
| Reload from the sbt build file | `sbt:_> reload` |
| Fetch dependencies | `sbt:_> update` |
| Create Docker image (requires SBT Native Packager plugin) | `sbt:_> Docker/publishLocal` |
| Create a distributable .zip file | `sbt:_> dist` |
| Run tests | `sbt:_> test` |
| Run incremental tests | `sbt:_> testQuick` |
| Run incremental tests continually | `sbt:_> ~testQuick` |
