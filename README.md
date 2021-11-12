# IVGS

Interfaced Videogame Specification (IVGS)
Motivation
There are too many unique processes in the game development field. So I wanted to create specifications that would not lead to creating more specifications, but encapsulate other specifications in a top-down functional way for individuals to create more reusable code during game development with an understandable language for the inclusion of code components and useful encapsulated defaults.

IVGS<IVGS Format Version>_<Specification  Class>_<Tags>_<Revision>(input1:encapsulated_specification, input2:format...)

Example Interface Specification Title:
IVGS1_SA1_H1_I1_1

Example Interface Specification Usage:
IVGS1_SA1_H1_I1_1(aspect:(1,2), image_format:png)

There is an additional Class Specification that is used to define the inherent use case and constraints of a Specification Class. The Specification Class also contains a living document for registering tags.

example Class Specification name:
IVGS1_SA1

IVGS Format Version - This specification layout may change in the future or the claim to a specification classes tag name may need to be yielded to another specification class in the future.

Specification Classes - These will own a global tag that is to be kept in this specification. This class specification will explain the general problem profile and the strategy for reusability within that problem domain. The Class will also keep track of related tags for children's specifications.
Example: An assembly of sprites to create a more complex asset. 

Tags - These tags should inherently be an attribute that is globally inherent to the problem domain as opposed to something that can be encapsulated. 

Example: H1 is for a simple humanoid and is registered as such in the Specification Class. 
  
