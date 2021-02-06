# Lab04 - SOEN 487 #

This is the Lab template for [Tutorial 4](https://github.com/SOEN487/T04).

You should watch the video for Tutorial 4 and clone [Tutorial 4](https://github.com/SOEN487/T04) before starting the lab. 

We encourage you to use either IntelliJ IDE or maven from command line in order to get the best support from our TAs.

## Existing Classes ##

[Calculator.java](https://github.com/SOEN487/Lab04/blob/main/src/main/java/com/example/soap/service/Calculator.java)

[CalculatorImpl.java](https://github.com/SOEN487/Lab04/blob/main/src/main/java/com/example/soap/service/CalculatorImpl.java)

Note: You will need to replace the sayHelloWorld and add the methods that are provided in your Lab instructions.

## IntelliJ Instructions ##

When importing the project in IntelliJ, you can go to File -> New -> Project From Existing Sources... and use the existing pom.xml file to initialize the project.

![Screenshot](img/intellij_existing.png)

Follow the tutorial on how to setup the service classes and the publisher. When they are done, right click on the ServicePublisher and choose Run main().

## Maven Instructions ##

    Run the folllowing commands in the associated project directory:

    Compile:
        mvn install
    Run (ServicePublisher)
        mvn exec:java -Ppublisher
    Clean:
        mvn clean

## Soap UI Testing ##

To test with SoapUI, run the program and click on new SOAP project. While ServicePublisher is still running, enter a project name and copy the WSDL url in the initial WSDL field.

![Screenshot](img/soapui.png)

You can now open requests from the navigator on the left, edit the message and send a SOAP request to the server to get a response. To submit the request, click on the green play button.

![Screenshot](img/soapui2.png)

