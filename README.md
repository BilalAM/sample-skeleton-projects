Sample Skeleton Projects
========================
[![Build Status](https://travis-ci.org/MSaifAsif/sample-skeleton-projects.svg?branch=master)](https://travis-ci.org/MSaifAsif/sample-skeleton-projects)

These projects are basic and easy to execute implementations of some of the popularly used frameworks and libraries out in the market and can be used to jump start your coding time by simply forking these projects or using them as reference and then building your application on top of them. The implementations range from advanced MVC frameworks such as Struts to small testing libraries like JUnit or pyUnit. 

**Note:** Projects not listed in the index table below are either in development phase or in debug mode and are not be relied on yet.

## <a name="list-index">List of implementation</a>
* [struts2 skeleton](#struts2skeleton)
* [struts1 skeleton](#struts1skeleton)
* [Jacoco Code coverage](#jacococoverage)
* [JBOSS RESTEasy service](#jboss-rest-service)
* [JSF skeleton](#jsf-skeleton)
* [Log4j logger](#log4j-logger)
* [Play skeleton](#play-skeleton)
* [Axis2 Webservice](#axis2-ws)
* [EJBs](#ejb-hw)
* [JPA using Hibernate](#jpa-hibernate)
* [JSoup](#jsoup-html)
* [Spark](#spark-mvc)
* [Servlet30HelloWorld](#servlet30-mvc)
* [pyUnit](#py-unit)
* [dotNET Webservice](#dotnet-ws)
* [How to contribute](#how-to-contrib)

## <a name="struts2skeleton">Struts2</a> [&#8593;](#list-index)
**Language:** Java

**Description:** A blank runnable web project based on the struts2 MVC architecture. The project comprises of a sample action class that will return success and display the resulting view (jsp file). The project can be run on any application server. Basic configurations including struts and log4j are also added for reference

**How to run:** Import the project as a maven project, build the war file using maven and place the war in the tomcat webapps folder. Once deployment is complete by tomcat, the sample MVC can be viewed at the URL `http://localhost:8080/Struts2HelloWorld/sample/GreetAction`

## <a name="struts1skeleton">Struts</a> [&#8593;](#list-index)
**Language:** Java

**Description:** A blank runnable web project based on the struts (The struts1) MVC architecture. The project comprises of a sample action class that will return success and display the resulting view (jsp file). The project can be run on any application server. Basic configurations including struts and log4j are also added for reference

**How to run:** Import the project as a maven project, build the war file using maven and place the war in the tomcat webapps folder. Once deployment is complete by tomcat, the sample MVC can be viewed at the URL `http://localhost:8080/StrutsHelloWorld/helloWorld.action`

## <a name="jacococoverage">JaCoco code coverage</a> [&#8593;](#list-index)
**Language:** Java

**Description:** A beginner level application implementing the jacoco maven plugin to cover code coverage of the JUNIT test cases within the application

**How to run:** Import the project as a maven project, run `mvn clean test` and jacoco will create a site project inside `{proj.dir}/target/site` with multiple files. Open the index.html in any browser and you can view and browse to the various classes and test cases and get a visual representation of the code coverage of the test cases written

## <a name="jboss-rest-service">JBOSS RESTEasy</a> [&#8593;](#list-index)
**Language:** Java

**Description:** An entry level application implementing the RESTEasy service of JBOSS. 

**How to run:** Import the project as a maven project, build the war file using maven and deploy this war in tomcat or Jboss application server. Once deployement is successful, you can view the service by opening any browser and navigate to the url `http://localhost:8080/RestEasyService/rest/greet/hello/Tenka`

## <a name="jsf-skeleton">JSF</a> [&#8593;](#list-index)
**Language:** Java

**Description:** An entry level MVC application built using the JSF framework. 

**How to run:** Import the project as a maven project, build the war file using maven and deploy this war in any JEE application server (Glassfish4 recommended). Once deployement is successful, you can view the landing page by opening any browser and navigate to the url `http://localhost:8080/JSFHelloWorld-0.0.1/welcome_page.xhtml`

## <a name="log4j-logger">Log4j</a> [&#8593;](#list-index)
**Language:** Java

**Description:** Basic implementation of how to create configure and use the logging capabilites provided by log4j.

**How to run:** Checkout the project to any directory and on the command prompt type `mvn clean test` and it will execute the test cases and a log will get printed on the console and the same log will be redirected to a log file namely `myApp.log` located at `${project_home}/logs`. The key point to understand is how to use the configuration file that is read by the log4j library. This file is located at `src/main/resources/log4j.properties`

## <a name="play-skeleton">Play MVC</a> [&#8593;](#list-index)
**Language:** Java & Scala

**Description:** Basic implementation of creating an MVC application using the Play framework.

**How to run:** Perhaps the most easy to use/configure MVC framework out there. To run the application, you need to have Play installed and available on the classpath. Once installed, checkout the project, and while standing inside the directory of the `PlayHelloWorld`, run the command `play` and you will enter inside the play terminal. Next, just type in `run` and play will compile and deploy your application on an embedded jetty server and you can view your application using the url `http://localhost:9000` or `http://localhost:9000/HelloWorld` (routes have been set for both URLs)

## <a name="axis2-ws">Axis2 Webservice</a> [&#8593;](#list-index)
**Language:** Java

**Description:** Basic implementation of creating an XML SOAP web service using Axis2. Note that this is just a web service implementation, to consume the web service, use any web service client like SOAPUI or you can create your own.

**How to run:** To run the project, checkout and deploy the war on tomcat7 application server. The wsdl will be available at the URL `http://localhost:8080/AxisWebserviceHelloWorld/services/CalculatorService?wsdl`. 

## <a name="ejb-hw">EJBs</a> [&#8593;](#list-index)
**Language:** Java

**Description:** Basic implementation of how to create, deploy and then retrieve a stateless session bean using the EJBs API via JNDI.

**How to run:** There are two parts on how to execute the project. First we need to build the project with `mvn clean install`. Next, copy the built war file into the deployements folder for the application server (project has been optimized and tested against wildfly8.2). Once deployed, now we need to retrieve this EJB via JNDI. For this, run the main method in the class `com.sample.client.StandAloneClient`. You can see the logs printed in the server logs. 

## <a name="jpa-hibernate">JPA using Hibernate ORM</a> [&#8593;](#list-index)
**Language:** Java

**Description:** Basic workflow of how to implement the Hibernate implementation of JPA. Hibernate is one of the powerfull, scalable, flexible and most used ORM framework used in the software industry.

**How to run:** Checkout the project and execute the MainRunner class that is located inside the package `com.main`. The application uses HSQLDB(http://hsqldb.org/) for carrying out CRUD operations so no DB is requiered to run the program, although you can direct it to your Database by simply changing the `hibernate.connection.url` in `hibernate.cfg.xml`. This is the configuration file used by hibernate to connect to your DB.  

## <a name="jsoup-html">Jsoup HTML parser</a> [&#8593;](#list-index)
**Language:** Java

**Description:** A dummy implementation of the Jsoup library to parse html documents.

**How to run:** Checkout the project and execute the command `mvn clean test`. Basic parsing have been implemented as Junit cases. Also there is a main method in the class `com.sample.one.MainRunner` that shows how to parse and retreive information via Jsoup for a particualr Html page on the web

## <a name="spark-mvc">Spark MVC</a> [&#8593;](#list-index)
**Language:** Java (JDK8)

**Description:** A skeleton implementation of an MVC application using the Spark framework. Another simple and easy to implement MVC framework that can be used to expose a set of REST calls quick and easy. Comes with an embedded server so no deployment is required.

**How to run:** Checkout the project and execute the command `mvn clean test`. Then simply run the main method located at `com.sampl.main.MainRunner` and the server will load up at `localhost:4567`. Navigate to the URL `localhost:4567/helloWorld` and you will see the logs in the console as well as a sample text being returned from the exposed method

## <a name="servlet30-mvc">Servlet/JSP</a> [&#8593;](#list-index)
**Language:** Java

**Description:** Basic implementation of an MVC architecture based on raw Servlets and JSPs. 

**How to run:** Checkout the project and execute the command `mvn clean install`. Deploy the generated war file in any application server (Tomcat 7) and then navigate to the page `http://localhost:8080/Servlet30HelloWorld/helloServlet` and you will be greeted with a message from a compiled JSP.

## <a name="py-unit">pyUnit</a> [&#8593;](#list-index)
**Language:** Python

**Description:** Basic implementation of how to create unit tests for python2.7 using the built-in unit test library for the python language. 

**How to run:** Checkout the project to any directory and on the command prompt type `python cal_test.py` and it will execute the test cases and the result status of all the test cases will be displayed on the terminal

## <a name="dotnet-ws">.NET WebService</a> [&#8593;](#list-index)
**Language:** .NET Framework 4.0

**Description:** Basic implementation of creating a simple SOAP web service using .NET Framework.

**How to run:** Checkout the project and deploy it. It automatically hosts the web service on a test server hosted on http://tempuri.org. The wsdl will be available at the URL `http://localhost:1672/Service1.asmx?wsdl`.

## <a name="how-to-contrib">How to contribute</a> [&#8593;](#list-index)

The project is open for contributions from everyone. If you want to contribute to the project, the best way is to 
* Check the issues page to see if any pending issue is left and fixable
* Fork the repo
* Add documented and tested code
* Open a pull request to the master branch
* Once reviewed, the pull request will be merged
* README.md will contain information of runnable projects ONLY. All other projects are either in dev or testing phase

Its always best to open a issue and discuss its possibility before writing up the code. I am always open for suggestions. Feel free to contact/contribute.
