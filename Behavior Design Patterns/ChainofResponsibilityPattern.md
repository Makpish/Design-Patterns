#Chain of Responsibility Pattern
##https://springframework.guru/gang-of-four-design-patterns/chain-of-responsibility-pattern/


- Avoid coupling the sender of a request to its receiver by giving more than one object a chance to handle the request. Chain the receiving objects and pass the request along the chain until an object handles it.

- What the Chain of Responsibility pattern states is – decouple the client who sends the request to the object that handles it. The solution is a list of handler objects, also known as responding objects each capable to deal with a specific nature of request. If one handler object can’t handle a request, it passes it to the next object in the chain. At the end of the chain, there will be one or more generic handler objects implementing default behavior for the request.
