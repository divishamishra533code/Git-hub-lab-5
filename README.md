# Spring Autowiring Demo using @Autowired

## Academic Purpose

This project is developed as part of an academic assignment to demonstrate Dependency Injection and Autowiring in the Spring Framework. It is intended for educational purposes only.

## Introduction

Spring Framework provides Dependency Injection (DI) to reduce tight coupling between classes. Autowiring allows Spring to automatically inject dependent objects. In this project, a Certification object is injected into a Student object using the @Autowired annotation without using the new keyword.

## Objective

* Understand Autowiring in Spring
* Implement Dependency Injection using @Autowired
* Learn annotation-based configuration

## Prerequisites

* Basic knowledge of Java
* Understanding of Spring Framework basics
* Knowledge of Dependency Injection

## Project Description

The application consists of two classes:

### Certification

* Fields: id, name, dateOfCompletion
* Managed by Spring using @Component

### Student

* Fields: id, name, gender
* Contains a Certification object
* Uses @Autowired for dependency injection

Spring automatically creates and links both objects using the IoC container.

## Technologies Used

* Java
* Spring Framework (spring-context)
* Maven

## Configuration

* @Configuration for configuration class
* @ComponentScan for scanning components
* @Component to create beans
* @Autowired to inject dependencies

## How It Works

1. Spring scans classes annotated with @Component
2. Beans are created and stored in the IoC container
3. @Autowired injects Certification into Student
4. Application retrieves Student bean and displays details

## How to Run

1. Clone the repository
2. Open in IntelliJ or Eclipse
3. Install Maven dependencies
4. Run the main class

## Sample Output

Student ID: 1
Student Name: Divisha
Gender: Female

--- Certification Details ---
Certification ID: 101
Certification Name: Java Programming
Date of Completion: 2025-03-10

## Key Concepts

* Inversion of Control (IoC)
* Dependency Injection (DI)
* Autowiring
* Spring IoC Container

## Conclusion

This project demonstrates how Spring simplifies dependency management using @Autowired. It eliminates manual object creation and promotes loose coupling, making applications easier to maintain.
