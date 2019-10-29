 Who is MrChecker?

MrChecker Test Framework in the end to end test automation framework written in Java. 
It is an automated testing framework for functional testing of web applications, API web services, Service Virtualization, Security and in coming future native mobile apps, and databases. All modules have tangible examples of how to build resilient integration test cases based on delivered functions. 

image::content.PNG["E2E Test Framework  for DevOps & Smart Automation", width="450", link="documentation/E2E_Test_Framework_for_DevOps_Smart_Automation_ver2/Slide4.PNG"]

==== Where MrChecker applies?

The main goal of MrChecker is to standardize the way we build BlackBox tests. It gives the possibility to have one common software standard in order to build: Component, Integration and System tests.

image::piramida.png["Test pyramis", width="450", link="documentation/E2E_Test_Framework_for_DevOps_Smart_Automation_ver2/Test_pyramid.png"]

A Test Engineer does not have access to the application source code in order to perform BlackBox tests, but he is able to attach his tests to any application interfaces, such as  - IP address - Domain Name - communication protocol - Command Line Interface.

MrChecker’s specification:

* Responsive Web Design application: Selenium Browser

* REST/SOAP: RestAssure

* Service Virtualization: Wiremock

* Database: JDBC drivers for SQL

* Security: RestAssure + RestAssure Security lib

* Standalone Java application: SWING

* Native mobile application for Android: Appium

==== Test stages

===== Unit test

A module is the smallest compilable unit of source code. It is often too small to be tested by the functional tests (black-box tests). However, it is the ideal candidate for white-box testing. White - box tests have to be performed as the first static tests (e.g. Lint and inspections), followed by dynamic tests in order to check boundaries, branches and paths. Usually, that kind of testing would require the enablement of stubs and special test tools. 

===== Component test

This is the black-box test of modules or groups of modules which represent certain functionalities. There are no rules about what could be called a component. Whatever a tester defines as a component, should make sense and be a testable unit. Components can be step by step integrated into the bigger components and tested as such. 

===== Integration test

Functions are tested by feeding them input and examining the output, and internal program structure is rarely considered. The software is step by step completed and tested by the tests covering a collaboration of modules or classes. The integration depends on the kind of system. For example, the steps could be as such: run the operating system first and gradually add one component after another, then check if the black-box tests still are running (the test cases will be extended together with every added component). The integration is done in the laboratory. It may be also completed by using simulators or emulators. Additionally, the input signals could be stimulated. 

===== Software / System test

System testing is a type of testing conducted on a complete integrated system to evaluate the system’s compliance with its specified requirements. This is a type of black-box testing of the complete software in the target system. The most important factor in the successful system testing is that the environmental conditions for the software have to be as realistic as possible (complete original hardware in the destination environment).