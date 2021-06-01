# Red Hat Data Grid 8 Simple Tutorials  

This is a collection of simple tutorials that explain how to use Data Grid in a straightforward way.

## Building Tutorials

To build the tutorials you need:

- JDK 8
- Apache Maven 3.x

Compile and run each tutorial by invoking the following commands from its folder:

```bash
mvn -s /path/to/maven-settings.xml clean package
mvn -s /path/to/maven-settings.xml exec:exec
```

Note that the `maven-settings.xml` file is available in the root directory of
this repository.

## Remote cache tutorials

Tutorials that use remote caches require at least one Data Grid Server running locally.

Download the server distribution from the [Red Hat customer portal](https://access.redhat.com/jbossnetwork/restricted/listSoftware.html?product=data.grid&downloadType=distributions) and run:

```bash
./bin/cli.sh user create admin -p "changeme"
./bin/server.sh
```

**By default, Data Grid Server 8.2 requires authentication and requires users to have access permissions.** 
Creating a user named `admin` gives you full access permissions for Data Grid Server.
Find more details about setting up authorization roles in [Creating and Modifying Users](https://access.redhat.com/documentation/en-us/red_hat_data_grid/8.2/html/data_grid_server_guide/start_server#creating-users_quickstart)
