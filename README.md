# Private-Research-Containers

This project was developed in partnership with BMD Software company and had as its primary objective the search for existing technological solutions that aim to improve the collaborative factor in the research area, and consequently create a new solution.

As a result, a web platform was developed to enable the creation of virtual and collaborative spaces for sharing and analyzing clinical research data. It is a system that meets strong security requirements, including two-factor authentication and protection of data copy by its users.

### System Implementation

![alt text](https://github.com/gabrielpatricio/Private-Research-Containers/blob/master/prcarch.png)

### Demonstration
##### Authentication and Authorization System

The platform redirects the user to a login page to provide access to their profile and resources. If the user does not already have an account on the platform, it can be registered if providing parameters such as username, password, and email. After registration, the Regular User profile is assigned.

![alt text](https://github.com/gabrielpatricio/Private-Research-Containers/blob/master/prcAuthDemo.gif)

##### Project and User Management

Regarding project and user management actions, the platform provides endpoints to CRUD methods relating to projects, users, and relationships between them, all of which can be done intuitively in the platform GUI.

![alt text](https://github.com/gabrielpatricio/Private-Research-Containers/blob/master/projusermanag.gif)

##### Highly customized integration with container-based applications

The integration with Docker is responsible for making this system so parameterizable and flexible. The use of Docker daemon gives it great flexibility in terms of the diversity of applications provided per project, offering the possibility of creating a flexible and customized virtual research environment.

The data created, modified or analyzed using a platform application can be either private or shared with other users, depending on application settings when integrated with the platform.

![alt text](https://github.com/gabrielpatricio/Private-Research-Containers/blob/master/highlycustom.gif)

##### RBAC System 

**Regular User** - A user who registers on the platform has this profile assigned by default. This profile allows you to browse the projects where you are inserted, using its applications and services.
* A Regular User may have associated one or more roles and they will specify which area of development of the project they will have access to and their permissions.

**Project Manager** - This user is in charge of managing projects, ie adding new members to it and providing new applications.

**Platform Administrator** - This user is in charge of assigning profiles to the platform users, and has access to the server, technical problems related to it are solved by this user.

![alt text](https://github.com/gabrielpatricio/Private-Research-Containers/blob/master/rbacsys.gif)

### Library Dependencies


[Java Docker API Client](https://github.com/docker-java/docker-java)

[Keycloak API](https://www.keycloak.org/docs-api/8.0/javadocs/index.html)

[Java Persistence API](https://docs.oracle.com/javaee/7/api/javax/persistence/package-summary.html)

[WebDav Client](https://github.com/lookfirst/sardine)
