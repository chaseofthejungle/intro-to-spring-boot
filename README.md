# Intro to Spring Boot
  
#### Table of Contents
  
1. [How Spring Boot Differs from Spring](#differences)
2. [Spring Boot Actuator](#actuator)
3. [Spring Initialzr](#initialzr)
4. [Supplemental Resources](#supplemental)
  
<hr />
  
**Description/Overview:** Spring Boot is an open source framework of libraries for the setup, programming, configuration, and deployment of Java microservice applications. Examples of Spring Boot features include diagnostic checks, production-ready metrics, customizable startup configurations, and embedded app servers (e.g., Jetty, Tomcat, Undertow). No code or XML generation is necessary to create Spring Boot projects, and best configurations for projects are automatically determined (and manually adjustable, as desired or needed).
  
<hr />
  
## 1. <a name="differences">How Spring Boot Differs from Spring</a>

Spring is a configuration framework that empowers enterprise Java app developers with flexible, ready-to-use controls and boilerplate code that make apps quicker and simpler to setup, allowing developers to focus more on the other aspects of development. The Spring Boot framework is assembled 'on top of' it, with extra features (such as additional configuration tools) that make generating stand-alone/autonomous apps even *more* convenient to setup and configure. 
  
<hr />
  
## 2. <a name="actuator">Spring Boot Actuator</a>
  
This module includes production-environment tools for manging and monitoring Spring Boot app processes and performance. Insights into properties, metrics, diagnostics, and other characteristics are determined via the exposing of endpoints (e.g., '/actuator/metrics', '/actuator/info', /'actuator/health'). Spring Boot Actuator can be configured and integrated with third-party tools/technologies.
  
<hr />
  
## 3. <a name="initialzr">Spring Initialzr</a>
  
To create a simple RESTful Spring Boot web app using [Spring Initialzr](https://start.spring.io/): Add the dependency `spring-boot-starter-web` to a build.gradle or pom.xml file. Next, develop a controller class (using the annotation `@RestController`) and then a request mapping method using the relevant annotations (`@PostMapping`, `@GetMapping`). As an example:

```
@RestController
@RequestMapping("/api")  
public class SampleController {  
    @GetMapping("/sample")  
    public String printGreeting() {  
        return "Your map has been received!";  
    }  
}  
```

Use of either Spring Initialzr (or a similar tool) or manual typing/specification by the developer will be assumed for further examples in this guide involving adding dependencies.
  
<hr />
  
## 4. <a name="supplemental">Supplemental Resources</a>
  
* *[Official Spring Boot Website](https://spring.io/projects/spring-boot)*
* *[Java Data Structure Leetcode Interview Questions](https://github.com/chaseofthejungle/java-data-structure-leetcode-interview-questions)*
* *[Java Quick Reference Guide](https://github.com/chaseofthejungle/java-quick-reference-guide)*
