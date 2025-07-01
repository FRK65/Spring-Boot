
# 1. What is Spring Boot ? 

1. Spring Boot is a Java framework that makes it easier to create and run
Java applications.
2. It simplifies the configuration and setup process, allowing developers to focus more on writing code for their applications.
3. Spring Boot, a module of the Spring framework, facilitates Rapid Application Development (RAD) capabilities.
4. Spring Boot solve many developers problem
- Configurations
- Dependency Management
-  Embedded Server
-   And many more.

# 2. Why we choose Spring Boot over Spring ?

Spring Boot resolve limitation of Spring.
Spring Boot provide many advantages over normal spring framework 
- Easy to use- Remove boilerplate codes
- Production Ready applications- Metrix, Health Check and many features are designed for production ready application.
- Rapid Development- Opinionated approach and auto-configuration enable developers to quickly develop apps
- Provide Dependency Management- No need to manager separate dependencies manually.
- Autoconfiguration - Spring Boot AutoConfigure things by default.
- Embedded Server: provide tomat server by default.

# 3. Woring of Spring Boot.

1. Spring Boot starts by scanning the starter dependencies in pom.xml
2. Then download and auto-configure the module as you included in pom.xml
3. For example we have to create web application then we have to put **spring-boot-starter-web** dependency in pom.xml.
When we start the project spring boot downloads all the dependency required for web and configure the things like spring.

# 4. How Spring Boot Starts ?

1. Starts by calling main) method of you main class.
2. The run() method of SpringApplicaiton is called. This method starts the application by creating an application context and initializing it.
3. Once the application context is initialized, the run() method starts the application's embedded web server.
Ex.   
```java   
@SpringBootApplication
public class MyApplication {

  public static void main (String[] args) {

      SpringApplication.run(MyApplication.class,args);

  }
}
```
