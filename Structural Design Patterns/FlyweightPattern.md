#Flyweight Pattern
##https://springframework.guru/gang-of-four-design-patterns/flyweight-pattern/


- Use sharing to support large numbers of fine-grained objects efficiently.

- What this pattern says is that if an application requires a large number of fine-grained objects, share them instead o

- You can categorize the internal state into:

1. Intrinsic data: Information that is stored in the flyweight object. The information is independent of the flyweight’s context, thereby making it sharable. While applying the pattern, you take all of the objects that have the same intrinsic data and replace them with a single flyweight.

2. Extrinsic data: Information that depends on the flyweight’s context and hence cannot be shared. Client objects stores and computes extrinsic data and passes it to the flyweight when it needs it.