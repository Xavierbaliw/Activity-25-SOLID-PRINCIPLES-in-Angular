![SOLID PRINCIPLES in Angular](https://github.com/user-attachments/assets/f62466cb-7eba-4150-9fd0-7097b06a37a6)

## *Activity 25: SOLID PRINCIPLES in Angular*

When developing applications in Angular, maintaining a clean, modular, and scalable codebase can make a huge difference as your app grows in complexity. That’s where SOLID principles come into play. Originally introduced in object-oriented programming, these principles can also be applied in the world of Angular to help you write better, more maintainable code.

Here’s what SOLID stands for and how it applies to Angular development:

### *What Does SOLID Stand For?*

*S*: Single Responsibility Principle (SRP)

*O*: Open/Closed Principle (OCP)

*L*: Liskov Substitution Principle (LSP)

*I*: Interface Segregation Principle (ISP)

*D*: Dependency Inversion Principle (DIP)

Let’s break down each of these principles with Angular examples.

### 1. *Single Responsibility Principle (SRP)*

Definition: A class should have only one reason to change. This means a component, service, or module should have only one responsibility.

### *In Angular:*

Each component should focus on a single task, rather than trying to do everything. For instance, a form component should only handle form logic and not business logic or HTTP calls.

### *Example:*
![image](https://github.com/user-attachments/assets/d65e65f6-1016-44c9-a0b0-d7a573f7b98f)

Why it works: The component’s only job is to present data, while the service is responsible for retrieving that data.

### *2. Open/Closed Principle (OCP)*

Definition: Objects or entities should be open for extension but closed for modification. You should be able to add new functionality without changing existing code.

### *In Angular:*

Rather than modifying components or services when requirements change, you can extend their functionality through inheritance or by creating new services or modules.

### *Example:*
![image](https://github.com/user-attachments/assets/0f0061a2-163e-4979-9b87-356c3f0e8f0e)

Why it works: You can add new user types by creating new strategies without changing the existing service.

### 3. *Liskov Substitution Principle (LSP)*

Definition: Subtypes must be substitutable for their base types without affecting the correctness of the program.

### *In Angular:*

If you extend a component, service, or class, the derived class should be able to replace the base class without breaking functionality.

### *Example:*

![image](https://github.com/user-attachments/assets/1bfe83df-bf05-44f2-8f6d-10df0a6d6fd2)

Why it works: If you switch out BaseLogger for CustomLogger, the application will still work as expected.

### 4. *Interface Segregation Principle (ISP)*
Definition: Clients should not be forced to depend on interfaces they don’t use. In Angular, this applies to services and how components interact with them.

### *In Angular:*
Create smaller, focused services instead of one large service that tries to do everything. This ensures that your components or services only use what they need.

### *Example:*
![image](https://github.com/user-attachments/assets/12e98677-0b3b-4eea-94e1-2fdd6d62a690)

Why it works: Each service now has a clear, focused responsibility, making it easier to test and maintain.

### *5. Dependency Inversion Principle (DIP)*

Definition: High-level modules should not depend on low-level modules. Both should depend on abstractions.

### *In Angular:*

Use Angular’s dependency injection to inject dependencies at runtime, rather than hardcoding them.

### *Example:*
![image](https://github.com/user-attachments/assets/6d13c5b8-413d-4b8d-9f66-483f8cce92c6)

Why it works: You can easily replace the ApiService with another implementation, such as a mock API during testing, without modifying ProductService.

### *Conclusion*

The SOLID principles aren’t just for traditional object-oriented programming; they can also make your Angular apps easier to maintain, scale, and test. By following these principles, your code becomes more modular, readable, and flexible. Whether you’re working on components, services, or modules, keeping these principles in mind will help you avoid a messy and tightly-coupled codebase.

Remember, writing good code is not just about functionality — it’s about writing code that’s easy to understand, extend, and maintain. By applying the SOLID principles, you’ll create code that stands the test of time (and growing feature requests).

*REFERENCES :* https://medium.com/@mrengith/the-solid-principles-in-angular-a-guide-to-cleaner-scalable-code-68c74a016338
