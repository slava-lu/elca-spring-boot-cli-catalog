# Elca Spring Boot Project Catalog
## Description

The ELCA Spring Boot Project Catalog provides a collection of pre-configured Spring Boot projects (boilerplates)
to help you quickly bootstrap new applications or add functionality to existing ones using the Spring CLI.

## Available projects

1. **ecla-starter**. Contains essential dependencies that are useful in every project.
2. **ecla-web**. Includes dependencies for building a REST API server.

## Prerequisites
* Java Development Kit (JDK) 17 or higher.
* Spring CLI installed on your system. Installation instruction: https://docs.spring.io/spring-boot/installing.html#getting-started.installing.cli


## How to use

* Ensure that the Spring CLI is installed and available in your system's PATH: `spring version`
* Add the ELCA catalog to the Spring CLI by running: `spring project-catalog add elca https://github.com/slava-lu/elca-spring-boot-cli-catalog`,
  Here, _elca_ is an arbitrary name you assign to the catalog.
* Check that the catalog has been registered properly: `spring project-catalog list`. You should see the catalog with the name _elca_ in the output.
* To see the projects available in the Spring CLI, run: `spring project list`. You may also see a number of default projects that come with the Spring CLI.
* Create a new project using the **elca-starter** project first: `spring boot new my-app elca-starter`. This command will create a new project in the _my-app_ directory. 
* Navigate to your project directory: `cd my-app`. Add additional features by merging other projects from the catalog. 
For example, to add REST API server capabilities: `spring boot add elca-web`.

## Additional info
To find out more information about Spring CLI tool ge to https://docs.spring.io/spring-cli/reference/index.html
