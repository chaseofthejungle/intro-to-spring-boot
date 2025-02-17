# Intro to Spring Boot
**Description/Overview:** Spring Boot is an open source framework of libraries for the setup, programming, configuration, and deployment of Java microservice applications. Examples of Spring Boot features include diagnostic checks, production-ready metrics, customizable startup configurations, and embedded app servers (e.g., Jetty, Tomcat, Undertow). No code or XML generation is necessary to create Spring Boot projects, and best configurations for projects are automatically determined (and manually adjustable, as desired or needed).
  
**How does Spring Boot differ from Spring?**: Spring is a configuration framework that empowers enterprise Java app developers with flexible, ready-to-use controls and boilerplate code that make apps quicker and simpler to setup, allowing developers to focus more on the other aspects of development. The Spring Boot framework is assembled 'on top of' it, with extra features (such as additional configuration tools) that make generating stand-alone/autonomous apps even *more* convenient to setup and configure. 
  
**What is Spring Boot Actuator?:** This module includes production-environment tools for manging and monitoring Spring Boot app processes and performance. Insights into properties, metrics, diagnostics, and other characteristics are determined via the exposing of endpoints (e.g., '/actuator/metrics', '/actuator/info', /'actuator/health'). Spring Boot Actuator can be configured and integrated with third-party tools/technologies.

**To create a simple RESTful Spring Boot web app using [Spring Initialzr](https://start.spring.io/):** Add the dependency `spring-boot-starter-web` to a build.gradle or pom.xml file. Next, develop a controller class (using the annotation `@RestController`) and then a request mapping method using the relevant annotations (`@PostMapping`, `@GetMapping`). As an example:

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
  
TODO: Add initial numbered sections for document and a Table of Contents.
