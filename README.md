# OSLC-Lyo-Workshop-Projects
This project converts the original Lyo Workshop projects to use latest working version of Maven, and make it as a Dockerized applications from https://github.com/eclipse/lyo.docs

## Current Status
 - The Bugzilla Server can now be run as a Docker container - Please check [https://github.com/shameerkc/docker-bugzilla-sqlite](https://github.com/shameerkc/docker-bugzilla-sqlite) for more details on how to execute this
 - The example project has been setup as a Parent project.

## How to Build the project
 - Clone the Repo
 - Execute `mvn package` command in the parent folder. This will build the project in the corresponding folders.
 - The modules `ninacrm` and `Lab6` are prepared as war packages, which can be deployed using the lightweight `jetty` web server.
 - You can deploy the server using `mvn jetty:run` command in the child modules.

## Configurations
 - The Bugzilla server configurations are kept in bugz.properties file.

## Testing functionalities
 - If you use the Bugzilla container mentioned at [https://github.com/shameerkc/docker-bugzilla-sqlite](https://github.com/shameerkc/docker-bugzilla-sqlite), it will deploy Bugzilla at [http://localhost:8089/bugzilla/](http://localhost:8089/bugzilla/)
 - The default username is `admin` and password is `password`
 - The `ninacrm` module can be accessed using [http://localhost:8181/ninacrm/](http://localhost:8181/ninacrm/)
 - The `Lab6` module can be accessed using [http://localhost:8080/OSLC4JBugzilla/](http://localhost:8080/OSLC4JBugzilla/)

## Further References
 - Original project at [https://github.com/eclipse/lyo.docs](https://github.com/eclipse/lyo.docs)

 