# Red Hat Data Grid 8 Simple Tutorials  

This is a collection of simple tutorials that explain how to use certain
features of Red Hat Data Grid in the most straightforward way possible.

## Red Hat Data Grid Server tutorials

Several tutorials use remote caches and require a locally running Red Hat Data Grid Server.

Download the server from the [Red Hat customer portal](https://access.redhat.com/jbossnetwork/restricted/listSoftware.html?product=data.grid&downloadType=distributions) and run
from the downloaded files:

```bash
./bin/cli.sh user create admin -p "password"
./bin/server.sh
```
*IMPORTANT:* 
**Red Hat Data Grid Server requires authentication and authorization by default.** 
Creating a user named `admin` gives you administrative access to Red Hat Data Grid Server.
You can find more details about users and permissions in [Creating and Modifying Users](https://infinispan.org/docs/stable/titles/server/server.html#creating-users_quickstart)

## Building Tutorials

In order to build the tutorials you will need

- JDK 8
- Apache Maven 3.x
- Some examples use the Red Hat Data Grid Server. Download the server and run `bin/server.sh` from the installation directory

You can compile and run each individual tutorial by changing to its folder
and invoking:

```bash
mvn -s /path/to/maven-settings.xml clean package
mvn -s /path/to/maven-settings.xml exec:exec
```

Note that the `maven-settings.xml` file is available in the root directory of
this repository.
