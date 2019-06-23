# Identity Provider Group Mapper

This module allows to configure a identity provider claim mapper that sync the user's groups received from an external IdP into the Keycloak groups.

## Build

To build this module you will need:

* Java JDK 1.8
* Apache Maven 3

From command line you must run the following command to build the module:

> ``mvn clean package``

The module JAR will be available at ``target`` folder created by Maven inside the project folder.

## Installation

To install this module you must follow the instructions available at the [Keycloak documentation](https://www.keycloak.org/docs/latest/server_development/index.html#registering-provider-implementations) using the JAR built from last section of this document.

## Debug

To debug this module while developing you must enable the Keycloak debug mode. For this you must run the **standalone** script (``standalone.sh``, ``standalone.bat``) with the ``--debug <port>`` parameter. The ``port`` will be used by the debugger to connect remotely with Wildfly JVM.

For example, to enable Keycloak debug mode listening the port 8100 the standalone script must be like this (in Windows):

> ``standalone.bat --debug 8100`` 