# auto-bean-info
Automatically create a BeanInfo for all your @Entity and @MappedSuperclass and super classes and interfaces, to speed up class lookup when a JPA application starts.

# Usage

## With Maven

Add the repository to your pom.xml:

```
  <repositories>
    <repository>
      <id>auto-bean-info-repo</id>
      <name>GitHub Maven Packages</name>
      <url>https://maven.pkg.github.com/SimoneGianni/auto-bean-info</url>
    </repository>
  </repositories>
```

Add the dependency:

```
  <dependency>
    <groupId>it.semeru</groupId>
    <artifactId>auto-bean-info</artifactId>
    <version>0.0.1</version>
  </dependency>
```

Done. Next time your project builds, empty but existing BeanInfo will be generated, avoiding endless classpath scans.
