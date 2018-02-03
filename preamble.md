# EVE ESI (EVE Swagger Interface) auto-generated client

This client is auto-generated by the Swagger codegen maven plugin.

The auto-generated instructions in the installation are appended below but are not quite correct.  Please use the following instructions instead.

## Using the Library

A regular release of this library is deposited in [Maven Central](https://search.maven.org/).  Releases of the library are versioned by build date of the form `YYYYMMDD`.

For maven, add this dependency to your project's POM (substitute YYYYMMDD as appropriate):

```xml
<dependency>
    <groupId>enterprises.orbital.eve.esi</groupId>
    <artifactId>client</artifactId>
    <version>1.0.0.YYYYMMDD</version>
    <scope>compile</scope>
</dependency>
```

For gradle, add this dependency to your project's build file (substitute YYYYMMDD as appropriate):

```groovy
compile "enterprises.orbital.eve.esi:client:1.0.0.YYYYMMDD"
```

For everyone else, you'll need to first build the library with Maven as described below, then manually install the following JARs in the appropriate places (substitute YYYYMMDD as appropriate):

* target/eve-esi-client-1.0.0.YYYYMMDD.jar
* target/lib/*.jar

## Building the Library

The library should build cleanly out of the box with Maven as follows (we assume Java 1.8):

    mvn clean package

The `package` build phase includes a final assembly script which moves documentation to the correct location and builds this README file.

The library is always built based on the latest online Swagger specification for the EVE Swagger Interface.  You can build off of a downloaded specification instead by changing the `inputSpec` property of the `generate` goal in the POM file.

# Auto-Generated Installation Instructions
