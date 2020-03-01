# auto-bean-info
Automatically create a BeanInfo for all your @Entity and @MappedSuperclass and super classes and interfaces, to speed up class lookup when a JPA application starts.

# Usage

Deployed to both Github packages and a public S3 based repo.

## With Maven on public repository

Add the repository to your pom.xml:

```
  <repositories>
    <repository>
      <id>auto-bean-info-repo</id>
      <name>Public repo</name>
      <url>http://simonegianni-maven-repo.s3-website.eu-central-1.amazonaws.com/release</url>
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

## With Maven on Github packages

Make sure Github packages is configured on your Maven, see https://help.github.com/en/packages/using-github-packages-with-your-projects-ecosystem/configuring-apache-maven-for-use-with-github-packages

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
