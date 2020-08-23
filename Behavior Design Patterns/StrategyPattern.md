#Strategy Pattern
##https://springframework.guru/gang-of-four-design-patterns/strategy-pattern/


- “Define a family of algorithms, encapsulate each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients that use it."

- Using the Strategy pattern, we define a set of related algorithm and encapsulate them in classes separated from the host class (Encryptor). Clients can choose the algorithm to use at run time. By doing so, we can easily add a new algorithm or remove an existing one without modifying the other existing algorithms or the host class. Each of the algorithm classes adhere to the Single Responsibility principle, another SOLID principle as they will only be concerned with encrypting data with a specific algorithm, which is currently lacking in our Encryptor class. In addition, with smaller algorithm classes, unit testing becomes easier to focus on testing one particular situation.