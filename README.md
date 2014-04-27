# ReactiveMongo Extensions

This is a library providing DAO and DSL support for ReactiveMongo. The goal of *ReactiveMongo Extensions* is to provide all the necessary tools for ReactiveMongo other than the core functionality.

[![Build Status](https://travis-ci.org/fehmicansaglam/reactivemongo-extensions.svg?branch=master)](https://travis-ci.org/fehmicansaglam/reactivemongo-extensions)

## Using ReactiveMongo Extensions in your project

The latest release is 0.11.0.0-SNAPSHOT which is compatible with ReactiveMongo 0.11.0-SNAPSHOT.
The general format is that release a.b.c.d is compatible with ReactiveMongo a.b.c.

Note: Only available for scala 2.10.

If you use SBT, you just have to edit build.sbt and add the following:

```scala
resolvers += "Sonatype Snapshots" at "http://oss.sonatype.org/content/repositories/snapshots/"

libraryDependencies ++= Seq(
  "net.fehmicansaglam" %% "reactivemongo-extensions" % "0.11.0.0-SNAPSHOT"
)
```

## Contributions
Contributions are always welcome. Good ways to contribute include:

* Raising bugs and feature requests
* Fixing bugs
* Improving the performance
* Adding to the documentation

## Introduction

 *ReactiveMongo Extensions* currently provides two DAO types, which are [BsonDao](src/main/scala/dao/BsonDao.scala) and [JsonDao](src/main/scala/dao/JsonDao.scala). You may want to check test specifications for possible use cases. Both of the DAOs have similar APIs. Some of them are ```find```, ```findOne```, ```findById```, ```insert```, ```updateById```, ```count```, ```foreach```, ```fold```...
 
There also DSL helpers for each DAO type, which are [BsonDsl](src/main/scala/dsl/BsonDsl.scala) and [JsonDsl](src/main/scala/dsl/JsonDsl.scala). DSL helpers provide utilities to easily construct JSON or BSON queries. 

[BSON DAO](guide/bsondao.md)

[BSON DSL](guide/bsondsl.md)

[JSON DAO](guide/jsondao.md)

[JSON DSL](guide/bsondao.md)
