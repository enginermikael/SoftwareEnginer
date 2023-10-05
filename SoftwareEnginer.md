# Software Engineering

## Software Architecture

## 

### What is Software Architecture?

Describes how an application is built, including its components, how they interact with each other, the environment in which they operate, and so on.

### What does a Software Architect do?

An expert developer who designs software solutions from scratch, making high-level decisions about each step of the process, including technical standards, tools, design principles, platforms to be used, etc., leading a team of engineers to create the product Final.

### Software Architecture Levels

The architecture can be done at several `levels` of abstractions. The level influences the importance of the required skills. Since there are many possible categorizations, my favorite segmentation includes these 3 levels:

- #### Application Level:
  
   The lowest level of architecture. Focus on a single application. Very detailed and low-level design. Communication usually occurs within a development team.

- #### Solution Level:
  
   The middle level of architecture. Focus on one or more applications that meet a business need (business solution). Some high-end designs, but mostly low-end. Communication occurs between multiple development teams.

- #### Business Level:
  
   The highest level of architecture. Focus on multiple solutions. High-level abstract design, which needs to be detailed by solution or application architects. Communication occurs throughout the organization.

### Responsibilities of a Software Architect

To understand the necessary skills an architect needs, we first need to understand typical activities. The following list contains, from my perspective, the most important activities:

- Define and decide the technology and development platform.

- Define development standards, e.g. coding standards, tools, review processes, testing approach, etc.

- Support the identification and understanding of business requirements.

- Design systems and make decisions based on requirements.

- Document and communicate architectural definitions, designs and decisions.

- Check and review architecture and code, for example, check whether defined standards and coding standards are implemented correctly.

- Collaborate with other architects and stakeholders.

- Train and consult developers.

- Ensure that as implementation occurs, the architecture is being followed.

- Play a key role in code review.

- Detail and refine top-level design to bottom-level design.

***Note: Architecture is a continuous activity, especially when applied to agile software development. Therefore, these activities are carried out continuously.***

### Important Skills

### Clean Code Principles

Clean code is code that is easy to read, understand and maintain. It follows a set of principles designed to make code more readable, testable, and less error-prone. Some of the key principles of clean code include:

- **Clarity:** The code must be easy to read and understand.

- **Simplicity:** The code should be as simple as possible, avoiding unnecessary complexity.

- **Comments:** Comments should be used sparingly and only when necessary to explain complex or non-obvious code.

- **Nomenclature:** Variables, functions and classes must have meaningful and descriptive names.

- **Formatting:** Code must be formatted consistently to improve readability.

- **Functionality:** The code must be organized into small, single-purpose functions and classes.

- **Error Handling:** the code must handle errors in a consistent and predictable manner.

- **Test:** The code must be testable and have high test coverage.

- **Reusability:** The code must be designed to be reusable and modular.

- **Performance:** code must be designed to be efficient and high-performance.

- **Being Consistent:** Being consistent refers to maintaining a consistent standard. This may include using consistent naming conventions, data structures, and interfaces throughout the system, as well as adhering to established design principles and best practices. Consistency can help make the system more maintainable, understandable, and extensible.

- **Indentation and Code Styling:** Indentation is the practice of using white space to visually group related lines of code, making the code structure easier to read and understand. Code style refers to the conventions and guidelines used to format and structure code, such as naming conventions, comments, and the use of white space.
  
   Having an indentation and a consistent code style These can help make code more readable and understandable, which can improve system maintainability.
  
  - **Keep It Small:** You should design and implement small, focused components that serve a specific purpose, rather than large, monolithic components that try to do it all. This can help improve system maintainability and scalability by making individual components easier to understand, test, and modify.
  
  - **Pure Functions:** A pure function is a specific type of function that meets the following criteria:
    
    - Takes some input, known as arguments, and returns a value or output.
    
    - Does not cause observable side effects, such as modification of the system state or interaction with external resources.
    
    - Given the same input, it will always return the same output.
    
    - It does not depend on any state or variable that is outside its scope.
      
      Pure functions are considered more predictable and easier to test, as their behavior is determined exclusively by the input they receive and their internal logic. They also make it easier to reason about a program's behavior, since the output of a pure function is not affected by any external factors. Pure functions are often used in functional programming, where they are considered a fundamental principle. They are also useful in concurrent and parallel programming as they are less prone to race conditions and other concurrency-related issues.
  
  - **Minimize Cyclomatic Complexity:** Cyclomatic complexity is a measure of the structural complexity of a program, which is determined by the number of linearly independent paths through a program's control flow. High cyclomatic complexity can make a program difficult to understand, test, and maintain, so it is often desirable to minimize it in the system architecture.
    
     Here are some ways to minimize cyclomatic complexity in system architecture:
  
  - Break down complex functions into smaller, simpler functions that perform specific tasks.
  
  - Use control structures, such as if-else statements and loops, in a consistent and predictable manner.
  
  - Use functional programming concepts and techniques, such as immutability and pure functions, to reduce the need for complex control flow.
  
  - Use design patterns, such as the state pattern, to simplify complex control flow.
  
  - Regularly review code and refactor it to simplify control flow.
  
  - Use static code analysis tools that can detect and report high cyclomatic complexity in code.
    
     By following these best practices, your system architecture will be more maintainable, testable, and less prone to errors.
  
  - **Avoid Passing Null Booleans:** Passing null or boolean values can lead to unexpected behavior and difficult-to-debug errors in a program. Here are some ways to avoid passing null or boolean values in the system architecture:
  
  - Use the Optional or Maybe types instead of null to indicate the absence of a value. This makes it clear when a value is missing and prevents null reference exceptions.
  
  - Use a default value for function arguments rather than allowing them to be null or boolean. This eliminates the need to check for null or Boolean values and reduces the potential for errors.
  
  - Use the Null Object pattern to replace null values with a special object that has a defined behavior. This eliminates the need to check for null values and makes the code more readable.
  
  - Use the ternary operator (?:) instead of if-else statements when working with booleans. This can make code more concise and easier to read.
  
  - Use the assert function to check the validity of the function's arguments and throw an exception if they are invalid.
  
  - **Keep Framework Code Away:** Keeping framework code apart refers to separating the application code from the framework code. By doing this, it becomes easier to independently maintain, test, and update the codebase and application structure.
    
     Here are some ways to keep framework code apart in the system architecture:
  1. Use an abstraction layer to separate application code from framework code. This allows application code to be written without needing to know the specifics of the framework.
  
  2. Use dependency injection to decouple application code from framework code. This allows application code to use the framework's functionality without having to directly instantiate the framework's objects.
  
  3. Avoid using framework-specific libraries or classes in your application code. This makes it easier to switch to a different framework in the future if necessary.
  
  4. Use a standard interface for the Application code interacts with the framework. This allows application code to be written without needing to know the specifics of the framework.
     
     5. Keep application and framework code in separate projects and/or repositories.
     
     6. By following these best practices, your system architecture will be more maintainable, testable, and less error-prone, and it will be easier to update or change the structure if necessary.
     - **Use correct constructs:** In the context of clean code principles, “use correct constructs” refers to using appropriate programming constructs, such as loops, conditionals, and functions, in a way that makes the code easy to understand , maintain and modify.
       
        When using correct constructs, the code must be organized logically and intuitively, making use of appropriate control flow statements and data structures to accomplish the task at hand. This also means that code should avoid using unnecessary or overly complex constructs that make the code more difficult to understand or reason about.
       
        Furthermore, correct constructs also mean using the right constructs for the right problem, for example, if you want to iterate over an array, use a for loop instead of recursion and also, you should avoid using global variables and instead Additionally, use function arguments and return values to pass data between different parts of the code.
       
        By using correct constructs, code will be more readable, easier to maintain, and less prone to bugs, making it easier for other developers to understand, debug, and extend the code.
     
     - **Keep Tests Independent:** Keeping tests independent helps ensure they are reliable, repeatable, and easy to maintain. When tests are independent, a change in one test will not affect the results of other tests.
       
        Here are some ways to keep tests independent across your system architecture:
     
     - Use dependency injection to decouple test code from application code. This allows tests to be run without the need to directly instantiate application objects.
     
     - Use mocks or stubs to isolate testing from external dependencies such as databases, APIs, or other services.
     
     - Use independent test data that does not depend on external data or states.
     
     - Use a testing framework that supports running tests in parallel, so that tests can be run independently of each other.
     
     - Use test-driven development (TDD), which involves writing tests before writing application code. This ensures that tests are independent and that code is written with testability in mind.
     
     - Avoid global state and shared mutable state as this may cause unexpected results.
     
     - - **Code by Act:** “Code by Actor” is a software development technique that encourages developers to organize their code around the actors or entities that interact with it. Actors can be users, systems, or processes that perform a specific role or function within the application. This approach helps create a clear separation of concerns, making code more modular, reusable, and easier to understand.
     
     - **Query Separation by Command:** Command-Query Separation (CQS) is a software design principle that separates the responsibilities of a method or function into two categories: commands and queries. Commands are methods that change the state of the system, while queries are methods that return information but do not change the state of the system.
     
     - **Avoid Hasty Abstractions:** Creating abstractions is an important part of software development, but creating too many abstractions or creating them too early can lead to unnecessary complexity and make code more difficult to understand and maintain.
       
        Here are some ways to avoid hasty abstractions in system architecture:
     
     - Understand the problem that needs to be solved before creating an abstraction.
     
     - Start with a simple solution and only create an abstraction when it becomes clear that the solution is becoming too complex.
     
     - Use code refactoring techniques to simplify code before creating an abstraction.
     
     - Avoid creating abstractions just for the sake of creating abstractions.
     
     - Use established design patterns and practices when creating abstractions, but don't force them into the code.
     
     - Use automated tests to ensure that the abstraction does not introduce new bugs or break existing functionality.
     
     - Create abstraction in a way that is easy to test, debug, and reason about.
     
     ### Programming Paradigms
     
     A programming paradigm is a fundamental style or approach to solving problems using a programming language. Different programming paradigms provide different ways of organizing and storing structure code and have different strengths and weaknesses. Some of the most common programming paradigms include:
     
     - Imperative programming
     - Functional programming
     - Object-oriented programming
     - Logic programming
     - Declarative programming
     
     #### Structured Programming
     
     Structured programming is a programming paradigm that emphasizes the use of structured control flow constructs, such as loops and conditional statements, to organize code into logical, easy-to-understand blocks. It is a way of writing computer programs that emphasizes the use of procedures and functions, as well as data structures, to organize code and make it easier to understand, debug, and maintain. The main idea behind structured programming is to break a program into smaller, manageable parts that can be easily understood, tested, and modified. This approach opposes the use of “goto” statements, which are considered unstructured and can lead to code that is difficult to read and maintain.
     
     #### Functional Programming
     
     Functional programming is a programming paradigm that emphasizes the use of pure functions and immutable data. It is a way of writing computer programs that emphasizes the use of functions and mathematical concepts, such as recursion, rather than using objects and classes as in object-oriented programming. In functional programming, functions are first-class citizens, meaning they can be passed as arguments to other functions and returned as values.
     
     Functional programming encourages immutability, meaning that once a variable is assigned a value, it cannot be changed. This can simplify code as it eliminates the need for state management and the bugs that can accompany it.
     
     ### Object Oriented Programming
     
     Object-oriented programming (OOP) is a programming paradigm that is based on the concept of “objects,” which are instances of classes. OOP is a way of organizing and structuring code based on the principles of encapsulation, inheritance and polymorphism.
     
     Encapsulation refers to the idea that the internal state of an object should be hidden and accessible only through its methods. This allows the object to control how its data is used and prevents external code from making invalid changes to the object's state.
     
     1. #### Model-Driven Design:
        
        Model-driven design (MDD) is a software development methodology in which the design of a system is represented by a set of models, and the models are used to drive system development. MDD is based on the idea that a system's design can be represented by a set of models, and that these models can be used to generate the system's code.
        
        The main advantage of using MDD is that it allows a clear separation of concerns between the design and implementation of a system. Models represent the design of the system, and code is generated from the models, which facilitates system maintenance and evolution. Additionally, MDD can also improve code quality as templates can be used to check for design errors and inconsistencies before code is generated.
        
        - **Domain Model:** A domain model is a representation of a specific area of knowledge or business that is used to model the objects and concepts within that domain and to capture the relationships and constraints between them. In object-oriented programming (OOP), a domain model is typically represented by a set of classes and interfaces, with each class or interface representing a specific concept or object within the domain.
          
          A domain model is used to provide a clear and consistent representation of the problem domain and to capture business requirements and system constraints. It is also used to guide system design and to ensure that the system accurately reflects the real-world problem it aims to solve.
        
        - **Anemic Models:** An anemic model, also known as an anemic domain model, is a type of domain model in which domain objects contain only data (attributes) and have no behavior. An anemic model often results in the use of data transfer objects (DTOs) and service layer to handle behavior.
          
          An anemic model is considered an anti-pattern in object-oriented programming (OOP) because it violates the principles of encapsulation and separation of concerns. In an anemic model, behavior is separated from data and is typically implemented in a separate service layer, which can lead to a code base that is complex, tightly coupled, and difficult to maintain.
        
        - **Layered Architectures:** A layered architecture is a software design pattern in which the functionality of a system is divided into a set of layers, with each layer having ing a specific responsibility and interacting with the layers above and below it. The main idea behind a layered architecture is to separate system concerns into distinct, independent layers, making code more modular, easier to understand, test, and modify.
          
               There are several types of layered architectures, but a common one is the three-tier architecture which consists of:
              
               - Presentation layer
               - Business layer
               - Data access layer
          
          - **Domain Language:** A domain language is a specific vocabulary and set of concepts used to describe and communicate about a specific area of knowledge or business. In software development, a domain language is used to model the objects and concepts within a specific domain and to capture the relationships and constraints between them.
            
            A domain language is used to provide a common understanding of the problem domain among all stakeholders, including developers, business analysts, and domain experts. It is also used to ensure that the software system accurately reflects the real-world problem it aims to solve.
          
          - **Class Invariants:** A class invariant is a set of conditions that must be true for any object of a class, at any time. In object-oriented programming (OOP), class invariants are used to define the valid states of an object and to ensure that the object always remains in a valid state.
            
            Class invariants are typically defined in the constructor of a class and are enforced through the use of private methods and data members that are used to validate the state of the object. They are also checked in the class's methods before and after any operation that might change the state of the object.
          2. #### Paradigm Features:
             
             Object-oriented programming (OOP) is a programming paradigm based on the concept of “objects,” which are instances of a class. OOP has several key features that distinguish it from other programming paradigms:
             
             1. Encapsulation
             
             2. Inheritance
             
             3. Polymorphism
             
             4. Abstraction
             
             5. Classes
             
             6. Objects
             
             7. Interfaces
             
             8. Dynamic linking
             
             9. Message passing
          - **Abstract Classes:** An abstract class is an object-oriented programming (OOP) class that cannot be instantiated. Instead, it serves as a template or template for other classes to inherit from. An abstract class can contain abstract and non-abstract methods (abstract methods are methods that do not have any implementation, they just have a signature).
            
            Abstract classes are used to provide a common interface and implementation for a group of related classes. They are also used to define common behavior that must be implemented by all subclasses. A subclass that inherits from an abstract class is called a concrete class and must provide an implementation for all abstract methods declared in the parent class.
          
          - **Concrete Classes:** A concrete class is an object-oriented programming (OOP) class that can be instantiated, which means objects can be created from it. A concrete class is a class that provides an implementation for all abstract methods declared in its parent class, if it inherits from an abstract class. A concrete class can also be a class that does not inherit from an abstract class, in which case it can have implementation for all its methods.
            
            Concrete classes are used to provide specific implementation details for a group of related classes that inherit from a common abstract class. They are also used to define unique behavior for a specific class. A concrete class can have its own methods and variables and can also override the methods of its parent class.
          
          - **Scope Visibility:** Scope visibility refers to the accessibility or visibility of variables, functions and other elements of a program, depending on the context in which they are defined. In object-oriented programming (OOP), scope visibility is controlled through the use of access modifiers such as “public”, “private” and “protected”.
            
            - Public: A public element can be accessed from anywhere in the program, both inside the class and outside it.
            - Private: A private element can only be accessed within the class in which it is defined. It is not accessible to other classes, even if they inherit from the class.
            - Protected: A protected element can only be accessed within the class and its subclasses.
          
          - **Interfaces:** In object-oriented programming (OOP), an interface is a contract or set of methods that a class must implement. It defines a set the common of methods that a class must provide, but does not provide implementation details. An interface can include method signatures and constants.
            
            Interfaces are used to define common behavior for a group of related classes and to provide a way for objects of different classes to be treated polymorphically. A class that implements an interface must provide an implementation for all methods declared in the interface. A class can implement multiple interfaces, but can only inherit from one base class.
