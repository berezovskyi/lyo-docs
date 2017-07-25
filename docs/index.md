# Welcome to Eclipse Lyo

> From https://projects.eclipse.org/projects/technology.lyo

The Eclipse Lyo project is focused on providing an SDK to enable adoption of OSLC specifications. [OSLC](https://oslc.github.io/) (Open Services for Lifecycle Collaboration) is an open community dedicated to reducing barriers for lifecycle tool integration. The community authors specifications for exposing lifecycle artifacts through uniform (REST) interfaces and relying on Internet and Linked Data standards.

OSLC's scope started with Application Lifecycle Management (ALM) and is expanding to include integrations across Product Lifecycle Management (PLM) and IT Service Management (ISM/DevOps), Lyo is designed to be a companion to the continuing specification efforts of the OSLC community. Its main purpose is to expand adoption of OSLC specifications and to enable the Eclipse community to easily build OSLC compliant tools.

## Getting started

Your POM file must refer to Lyo repositories:

```xml
<repositories>
    <repository>
        <id>lyo-releases</id>
        <name>Eclipse Lyo Releases</name>
        <url>https://repo.eclipse.org/content/repositories/lyo-releases/</url>
        <snapshots>
            <enabled>false</enabled>
        </snapshots>
    </repository>
    <repository>
        <id>lyo-snapshots</id>
        <name>Eclipse Lyo Snapshots</name>
        <url>https://repo.eclipse.org/content/repositories/lyo-snapshots/</url>
        <releases>
            <enabled>false</enabled>
        </releases>
    </repository>
</repositories>
```

Add the following dependencies to get the Lyo client ([javadoc](https://download.eclipse.org/lyo/docs/client/2.1.2/overview-summary.html)) support:

```
<dependency>
    <groupId>org.eclipse.lyo.clients</groupId>
    <artifactId>oslc-java-client</artifactId>
    <version>2.1.2</version>
</dependency>
```