# Reactive Relational Database Connectivity Service Provider Interface (R2DBC SPI) [![Build Status](https://travis-ci.org/r2dbc/r2dbc-spi.svg?branch=main)](https://travis-ci.org/r2dbc/r2dbc-spi) [![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.r2dbc/r2dbc-spi/badge.svg)](https://maven-badges.herokuapp.com/maven-central/io.r2dbc/r2dbc-spi)

The Reactive Relational Database Connectivity (R2DBC) project brings reactive programming APIs to relational databases.

## In a Nutshell

**Based on the Reactive Streams specification.** R2DBC is founded on the Reactive Streams specification, which provides a fully-reactive non-blocking API.

**Works with relational databases.** In contrast to the blocking nature of JDBC, R2DBC allows you to work with SQL databases using a reactive API.

**Supports scalable solutions.** With Reactive Streams, R2DBC enables you to move from the classic “one thread per connection” model to a more powerful and scalable approach.

**Provides an open specification.** R2DBC is an open specification and establishes a Service Provider Interface (SPI) for driver vendors to implement and clients to consume.

## Code of Conduct

This project is governed by the [R2DBC Code of Conduct](https://github.com/r2dbc/.github/blob/main/CODE_OF_CONDUCT.adoc). By participating, you are expected to uphold this code of conduct. Please report unacceptable behavior to [info@r2dbc.io](mailto:info@r2dbc.io).

### Maven configuration

Artifacts can be found on [Maven Central](https://search.maven.org/search?q=r2dbc-spi).

```xml
<dependency>
  <groupId>io.r2dbc</groupId>
  <artifactId>r2dbc-spi</artifactId>
  <version>${version}</version>
</dependency>
```

If you'd rather like the latest snapshots of the upcoming major version, use our Maven snapshot repository and declare the appropriate dependency version.

```xml
<dependency>
  <groupId>io.r2dbc</groupId>
  <artifactId>r2dbc-spi</artifactId>
  <version>${version}.BUILD-SNAPSHOT</version>
</dependency>

<repository>
  <id>spring-libs-snapshot</id>
  <name>Spring Snapshot Repository</name>
  <url>https://repo.spring.io/libs-snapshot</url>
</repository>
```

## Getting Help

Having trouble with R2DBC? We'd love to help!

* The R2DBC website https://r2dbc.io/ gives you an overview over the entire R2DBC eco-system.
* Check the [spec documentation](https://r2dbc.io/spec/0.8.1.RELEASE/spec/html/), and [Javadoc](https://r2dbc.io/spec/0.8.1.RELEASE/api/).
* If you are upgrading, check out the [changelog](https://r2dbc.io/spec/0.8.1.RELEASE/CHANGELOG.txt) for "new and noteworthy" features.
* Ask a question - we monitor [stackoverflow.com](https://stackoverflow.com) for questions
  tagged with [`r2dbc`](https://stackoverflow.com/tags/r2dbc). 
  You can also chat with the community on [Gitter](https://gitter.im/r2dbc/r2dbc).
* Report bugs with R2DBC SPI at [github.com/r2dbc/r2dbc-spi/issues](https://github.com/r2dbc/r2dbc-spi/issues).

## Reporting Issues

R2DBC uses GitHub as issue tracking system to record bugs and feature requests. 
If you want to raise an issue, please follow the recommendations below:

* Before you log a bug, please search the [issue tracker](https://github.com/r2dbc/r2dbc-spi/issues) to see if someone has already reported the problem.
* If the issue doesn't already exist, [create a new issue](https://github.com/r2dbc/r2dbc-spi/issues/new).
* Please provide as much information as possible with the issue report, we like to know the version of R2DBC SPI that you are using and JVM version.
* If you need to paste code, or include a stack trace use Markdown ``` escapes before and after your text.
* If possible try to create a test-case or project that replicates the issue. 
Attach a link to your code or a compressed file containing your code.

## Building from Source

You don't need to build from source to use R2DBC SPI (binaries in Maven Central), but if you want to try out the latest and greatest, R2DBC SPI can be easily built with the
[maven wrapper](https://github.com/takari/maven-wrapper). You also need JDK 1.8 and Docker to run integration tests.

```bash
 $ ./mvnw clean install
```

If you want to build with the regular `mvn` command, you will need [Maven v3.5.0 or above](https://maven.apache.org/run-maven/index.html).

_Also see [CONTRIBUTING.adoc](https://github.com/r2dbc/.github/blob/main/CONTRIBUTING.adoc) if you wish to submit pull requests, and in particular please sign the [Contributor's Agreement](https://cla.pivotal.io/sign/reactor) before your first change, however trivial._

## License
This project is released under version 2.0 of the [Apache License][l].

[l]: https://www.apache.org/licenses/LICENSE-2.0
