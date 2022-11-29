# Full-Stack-Notes

Chapter 1 Setting Up the Environment and Tools – Backend

Apache Maven is a software project management tool that makes the software 
development process simpler and also unifies the development process.

The basis of Maven is the Project Object Model (POM). The POM is a pom.xml file that 
contains basic information about a project. There are also all the dependencies that Maven 
should download to be able to build a project.

Spring Initializer
•	a web-based tool that's used to create Spring Boot projects.
Loggers
•	Logging can be used to monitor your application flow, 
•	Capture unexpected errors in your program code. 
•	The logger.info method prints a logging message in the console. Logging messages 
•	There are (7) different logging levels: TRACE, DEBUG, INFO, WARN, ERROR, FATAL, OFF
•	Logging levels are set in the application.properties file

The Spring Boot DevTools dependency provides us with the Spring Boot developer 
tools, which provide automatic restart functionality. It makes development much 
faster because the application is automatically restarted when changes have been 
saved. The web starter pack is a base for full stack development and provides an 
embedded Tomcat server.

Chapter 2
DI is a software development technique where we can create objects that depend on other 
objects. DI helps with interaction between classes but at the same time keeps the classes 
independent

Spring Boot scans your application classes and registers classes with certain annotations 
•	@Service
•	 @Repository 
•	@Controller
•	as Spring beans. These beans can then 
be injected using an @Autowired annotation:

A service is a class that can be used (this is the dependency).
• The client is a class that uses the dependency.
• The injector passes the dependency (the service) to the dependent class (the client)

Chapter 3

Object Relational Mapping (ORM) 
•	is a technique that allows you to fetch from and 
manipulate a database by using an object-oriented programming paradigm.
Java Persistent API (JPA ) 
•	provides object-relational mapping for Java developers. The 
JPA entity is a Java class that presents the structure of a database table.
•	Hibernate 
•	is the most popular Java-based JPA implementation and is used in Spring Boot 
by default. Hibernate is a mature product and is widely used in large-scale applications.
CrudRepository interface
•	CRUD functions (Create, Read, Update, Delete)
•	 Provides CRUD functionalities to our  
entity class.
•	@Autowired annotation is used to enable dependency injection
•	@Query annotation is used to create an SQL statement
•	Query staements should be written in the crud repository
•	@OneToMany annotation creates a relationship with one object to many of that object type
•	@ManyToOne annotation is sister to @OneToMany allowing multiple of an object type to belong to a single object
Chapter 4
Basics of REST

Representational State Transfer 

•	(REST) is an architectural style for creating web services.
•	 Stateless: The server doesn't hold any information about the client state.
•	 Client: The client and server act independently. The server does not send any 
information without a request from the client.
•	 Cacheable: Many clients often request the same resources; therefore, it is useful to 
cache responses in order to improve performance.
•	 Uniform interface: Requests from different clients look the same. Clients may 
include, for example, a browser, a Java application, and a mobile application.
•	Layered system: REST allows us to use a layered system architecture.
•	 Code on demand: This is an optional constraint.

Chapter 5
Spring Security
•	provides security services for Java-based web applications
HyperText Transfer Protocol 
•	(HTTP) basic security for all other endpoints

Securing your backend using a JWT
•	A JWT is a compact way to implement authentication in modern web applications.
•	Uniform Resource Locator (URL)
A JWT contains three different parts, separated by dots: xxxxx.yyyyy.zzzzz. These parts are 
broken up as follows:
• The first part (xxxxx) is the header that defines the type of the token and the 
hashing algorithm.
• The second part (yyyyy) is the payload that, typically, in the case of authentication, 
contains user information.
• The third part (zzzzz) is the signature that is used to verify that the token hasn't 
been changed along the way
cross-origin resource sharing (CORS) 
•	filter to our security configuration class. This is needed for the frontend, which is sending requests from the other origin.
Chapter 15 Deploying Your App
There are a number of cloud servers
•	Platform-as-a-Service (PaaS)
•	Amazon Web Services (AWS)
Deploying the backend
Java Archive (JAR) 
•	Easiest way to deploy a Spring Boot Application

 

![image](https://user-images.githubusercontent.com/61952712/204560913-31c74536-7547-4906-9b65-a4a18de940ce.png)
