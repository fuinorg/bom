# bom

> A **Super BOM** aligned with both [Quarkus](https://quarkus.io/) and [Spring Boot](https://spring.io/projects/spring-boot) BOMs — pick a single set of third‑party versions that works with either framework.

[![Java Maven Build](https://github.com/fuinorg/bom/actions/workflows/maven.yml/badge.svg)](https://github.com/fuinorg/bom/actions/workflows/maven.yml)
[![Maven Central](https://img.shields.io/maven-central/v/org.fuin/bom.svg)](https://central.sonatype.com/artifact/org.fuin/bom)
[![License: LGPL](https://img.shields.io/badge/License-LGPL-blue.svg)](http://www.fsf.org/licensing/licenses/lgpl.html)
[![Java](https://img.shields.io/badge/Java-17%2B-blue.svg)](https://adoptium.net/)

---

## Overview

This BOM defines the **lowest common denominator** for third‑party dependency versions used across [fuin.org](https://github.com/fuinorg/) libraries.

By importing it, you can:

- Build libraries that work with **Quarkus** and **Spring Boot** out of the box
- Avoid clashes between transitive dependency versions
- Stay aligned with the versions that both frameworks ship with

See [CHANGELOG.md](CHANGELOG.md) for the exact Quarkus and Spring Boot BOM revisions currently aligned.

## Usage

Import the BOM in your project's `dependencyManagement` section.

```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>org.fuin</groupId>
            <artifactId>bom</artifactId>
            <version>1.0.0</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```
