# Kafka Processor Template

> Template for Kafka Streams Processor project @okp4.

[![version](https://img.shields.io/github/v/release/okp4/template-kafka-processor?style=for-the-badge&logo=github)](https://github.com/okp4/template-kafka-processor/releases)
[![build](https://img.shields.io/github/workflow/status/okp4/template-kafka-processor/Build?label=build&style=for-the-badge&logo=github)](https://github.com/okp4/template-kafka-processor/actions/workflows/build.yml)
[![lint](https://img.shields.io/github/workflow/status/okp4/template-kafka-processor/Lint?label=lint&style=for-the-badge&logo=github)](https://github.com/okp4/template-kafka-processor/actions/workflows/lint.yml)
[![test](https://img.shields.io/github/workflow/status/okp4/template-kafka-processor/Test?label=test&style=for-the-badge&logo=github)](https://github.com/okp4/template-kafka-processor/actions/workflows/test.yml)
[![conventional commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=for-the-badge&logo=conventionalcommits)](https://conventionalcommits.org)
[![contributor covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/okp4/.github/blob/main/CODE_OF_CONDUCT.md)
[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg?style=for-the-badge)](https://opensource.org/licenses/BSD-3-Clause)

## Purpose

TBD

## Implementation

Implementation mainly relies on [Kafka Streams API](https://kafka.apache.org/documentation/streams), library to create
event-stream applications with the following features:

- no external dependency other than Kafka itself,
- simple and light library,
- fault-tolerant and scalable.

Moreover, this implementation:

- uses [Kotkin](https://kotlinlang.org/) as primary coding language,
- is as much as possible, lean, i.e. tries to minimize the dependencies to 3rd party libraries and the resulting package
  footprint.

## Build

This project targets the [JVM 11+](https://openjdk.java.net/), so be sure to have it available in your environment.

This project relies on the [Gradle](https://gradle.org/) build system.

If you are on windows then open a command line, go into the root directory and run:

```sh
.\gradlew build
```

If you are on linux/mac then open a terminal, go into the root directory and run:

```sh
./gradlew build
```

This command line produces 2 JAR files:

- a _regular_ JAR: `kafka-processor-X.Y.jar`
- a _fat_ JAR: `kafka-processor-X.Y-standalone.jar`

This last one is the one to use as it contains all the dependencies in it.

## You want to get involved? 😍

Please check out OKP4 health files :

- [Contributing](https://github.com/okp4/.github/blob/main/CONTRIBUTING.md)
- [Code of conduct](https://github.com/okp4/.github/blob/main/CODE_OF_CONDUCT.md)
