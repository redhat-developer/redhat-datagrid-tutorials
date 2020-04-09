# Red Hat Data Grid 8 Simple Tutorials

These tutorials demonstrate how to use Red Hat Data Grid 8 features.

## Prerequisites

To build the tutorials you need the following:

- JDK 8
- Apache Maven 3.x

Additionally, some tutorials interact with Data Grid server, which you can download from the [Red Hat customer portal](https://access.redhat.com/jbossnetwork/restricted/listSoftware.html?product=data.grid&downloadType=distributions).

## Running Tutorials

1. Open a terminal window and change to the directory of the tutorial you want to run.
2. Compile and run the tutorial as follows:

```bash
mvn -s /path/to/maven-settings.xml clean package
mvn -s /path/to/maven-settings.xml exec:exec
```

Note that the `maven-settings.xml` file is available in the root directory of
this repository.
