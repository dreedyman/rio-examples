# Rio Examples
This repository provides examples for developing dynamic services using the [Rio framework](https://github.com/dreedyman/Rio). The following examples are provided:

## Calculator Example
This example demonstrates a simple Calculator application that is composed of POJO services for each calculator function (add, subtract, multiply and divide).

Each calculator function is a deployable service, and the Calculator has a declared association to each service. The Calculator service becomes 'whole' when it discovers it's required services. The Calculator is a good example on the use of associations and how association based dependency injection can be used.

## Events Example
This example demonstrates the use of the Rio event framework to subscribe to and be notified of events. Both services in this example are implemented as beans, client access to the example is done using either a CLI or through a Service UI. The use of customized proxies is also shown in this example, as well as the use of Watches. The Service UI can be viewed by using a service-UI compatible browser.

## SpringBean Example
This example demonstrates a simple Spring application. Rio provides the capability to build dynamic applications using Spring. You can wire up your beans using Spring, and use Rio to turn a Spring bean into a dynamic service, with built-in management, fault detection and automated deployment.

## Tomcat Example
The Tomcat example demonstrates how to activate and manage an existing (external) technology using the Rio exec framework. In this example, Tomcat is installed, deployed and started. The environment is set allowing Tomcat to be managed by JMX.

The example also shows how a declarative watch can be used to monitor JMX managed attributes, and set thresholds for manage-able Tomcat attributes. Our example shows how the MBean for the thread pool that handles incoming Web requests can be observed.

Our example will create a Service Control Adapter (SCA) to activate and monitor a Tomcat instance. The example requires no coding, just configuration of the OperationalString.

## Workflow Example
This example demonstrates a simple application which uses a JavaSpace to process a workflow. The workflow is determined by setting states in an Entry. The workflow itself is based on an enumerated Java class, with states of NEW, OPEN, PENDING and CLOSED. Generic worker instances are configured to process Entry types that match a specific template corresponding to a workflow state.

