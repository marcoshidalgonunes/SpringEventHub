# SpringEventHub

This project is an adaptation of [Spring Cloud Stream with Azure Event Hubs](https://learn.microsoft.com/en-us/azure/developer/java/spring-framework/configure-spring-cloud-stream-binder-java-app-azure-event-hub) from [Spring Cloud Azure](https://learn.microsoft.com/en-us/azure/developer/java/spring-framework/) documentation. Basically, the configuration uses the newest yaml format.

## Setup

The official documentation is not clear about how to setup a local development environment for this application. So the requirements to run this applications are described below:

* [Install or update the Azure Developer CLI](https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/install-azd).
* Follows the instructions in [Azure authentication in Java development environments](https://learn.microsoft.com/en-us/azure/developer/java/sdk/identity-dev-env-auth#azure-cli-credential), according to the IDE used.
* In an Azure Subscription, create a Resource Group containing an Event Hub Namespace and a Storage Account.
* In the Event Hub Namespace create an Event Hub. A Basic SKU is enough for running this example.
> **Note**
> Event Hub Basic SKU allows only the default consumer group.
* Assign the roles "Azure Event Hubs Data Sender" and "Azure Event Hubs Data Receiver" to the account used to login in Azure.
* In the Storage Account create a container to be used as checkpoint store.
* Assign the role "Storage Account Data Contributor" to the account used to login in Azure.
* Edit the configuration to comply with the resources created in the steps above.

## Reference

### Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/3.1.5/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/3.1.5/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/3.1.5/reference/htmlsingle/index.html#web)
* [Spring Cloud Azure developer guide](https://aka.ms/spring/msdocs/developer-guide)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [Deploying a Spring Boot app to Azure](https://spring.io/guides/gs/spring-boot-for-azure/)

### Additional Links
These additional references should also help you:

* [Azure Samples](https://aka.ms/spring/samples)

