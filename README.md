# AOP Sample - Aspect-Oriented Programming Example in Spring Boot

This is a simple example project that demonstrates the usage of Aspect-Oriented Programming (AOP) in a Spring Boot application. AOP allows you to modularize cross-cutting concerns in your application, such as logging, security, and transaction management.

## Prerequisites

Before running the project, ensure that the following dependencies are installed:

- Java 8 or higher
- Gradle

## Getting Started

Follow the steps below to get started with the AOP Sample project:

1. Clone the repository:

   ```bash
   git clone https://github.com/gitshishirkarki/aop-sample.git
   ```

2. Navigate to the project directory:

   ```bash
   cd aop-sample
   ```

3. Build the project using Gradle:

   ```bash
   gradle clean build
   ```

4. Run the application:

   ```bash
   gradle bootRun
   ```

## Overview

The AOP Sample project demonstrates a simple scenario of logging method execution time using AOP. The application consists of the following components:

- **Aspect**: `ExecutionTimeLoggerAspect` is an aspect that captures the execution time of methods annotated with the `@LogExecutionTime` annotation.
- **Controller**: `ExampleController` contains sample methods that are annotated with `@LogExecutionTime` to log their execution time.
- **Service**: `ExampleService` is a service class called by the controller, containing the business logic for the example.
- **Annotation**: `@LogExecutionTime` is a custom annotation used to mark methods for which the execution time will be logged.

## Usage

To use AOP in your own Spring Boot project, follow these steps:

1. Create an aspect class with the necessary pointcut and advice methods. Annotate the aspect class with `@Aspect` to mark it as an aspect.

2. Define the pointcut expression to target the specific methods or packages you want to intercept.

3. Implement advice methods (e.g., `@Before`, `@After`, `@Around`) to define the actions to be taken before, after, or around the intercepted method execution.

4. Annotate the methods that you want to intercept with custom annotations.

5. Configure AOP in your Spring Boot application by enabling AspectJ auto-proxying. This can be done by using the appropriate configuration in your Gradle build file.

For a detailed explanation and more advanced features of AOP, refer to the documentation and tutorials available for Spring AOP.

## Contributing

Contributions are welcome! If you find any issues or want to enhance this example project, feel free to open a pull request or submit an issue.

## Acknowledgements

This project is based on the concepts and examples provided by the Spring Framework. Special thanks to the Spring community for their valuable resources and contributions.
