# Red Hat Datagrid 8 Simple Tutorials

This is a collection of simple tutorials that explain how to use certain
features of Red Hat Datagrid 8 in the most straightforward way possible.

In order to build the tutorials you will need

- JDK 8
- Apache Maven 3.x
- Some examples use the Red Hat Datagrid. 
Download the lastest server version and run `bin/server.sh` from the installation directory

You can compile and run each individual tutorial by changing to its folder
and invoking:

```bash
mvn -s /path/to/maven-settings.xml clean package
mvn -s /path/to/maven-settings.xml exec:exec
```

Note: `maven-settings.xml` can be found in the root of the repository.

Then, check the tutorial for a particular URL to interact with.
