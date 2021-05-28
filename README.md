# axon-framework-bom

Bill of Material for axon-framework libs

[![Build Status](https://github.com/holixon/axon-framework-bom/workflows/Development%20branches/badge.svg)](https://github.com/holixon/axon-framework-bom/actions)
[![sponsored](https://img.shields.io/badge/sponsoredBy-Holisticon-RED.svg)](https://holisticon.de/)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.holixon.axon/axon-framework-bom/badge.svg)](https://maven-badges.herokuapp.com/maven-central/io.holixon.axon/axon-framework-bom)

## Usage

Include this bom in your `dependencyManagement` section to get all framework libs in the correct matching version without explicitly mentioning them in
your `dependencies` declarations.

**Maven:**

```xml
<dependency>
  <groupId>io.holixon.axon</groupId>
  <artifactId>axon-framework-bom</artifactId>
  <version>4.5.1</version>
  <type>pom</type>
  <scope>import</scope>
</dependency>
```

**Gradle:**

```kotlin
dependencies {
  implementation(platform("io.holixon.axon:axon-framework-bom:4.5.1"))
}
```

## Notes

* Possible duplicate of <https://github.com/AxonIQ/axon-bom>
