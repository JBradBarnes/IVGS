# Interfaced Videogame Specification (IVGS)

## Motivation
There are too many unique processes in the game development field. So I wanted to create specifications that would not lead to creating more specifications, but encapsulate other specifications in a top-down functional way for individuals to create more reusable code during game development with an understandable language for the inclusion of code components and useful encapsulated defaults.

IVGS<IVGS Format Version>_<Specification  Class>_<Tags>_<Revision>(input1:encapsulated_specification, input2:format...)

###Example Interface Specification Title:
IVGS1_SA1_H1_I1_1

###Example Interface Specification Usage:
IVGS1_SA1_H1_I1_1(aspect:(1,2), image_format:png)

There is an additional Class Specification that is used to define the inherent use case and constraints of a Specification Class. The Specification Class also contains a living document for registering tags.

###Class Specification
example Class Specification name:
IVGS1_SA1

###IVGS Format Version - This specification layout may change in the future or the claim to a specification classes tag name may need to be yielded to another specification class in the future.

###Specification Classes - These will own a global tag that is to be kept in this specification. This class specification will explain the general problem profile and the strategy for reusability within that problem domain. The Class will also keep track of related tags for children's specifications.
Example: An assembly of sprites to create a more complex asset. 

###Tags - 
  These tags should inherently be an attribute that is globally inherent to the problem domain as opposed to something that can be encapsulated. 

####Example: 
  H1 is for a simple humanoid and is registered as such in the Specification Class. 
  
###Inputs - 
These should be used for functionally defining interfaced pieces that can be used within the specs such as constant, data formats, or nested specifications. All Inputs should be grouped with a suitable default.

####Constants Examples:
In defining a sprite assembly an overall aspect ratio could be (1,2) or one half as wide as tall, since that is the default in is not needed to be included in the specification inputs. IVGS1_SA1_H1_I1_1(image_format:jpg) 
A default unit could be one as defined as the systems float, but the unit could be overwritten as a functional spec with the inputs to use as pixels as opposed to the default of the systems dimensional float: IVGS1_SA1_H1_I1_1(image_format: jpg, units: px)
####Format Example:
-In defining a sprite assembly the default sprite image format is png, since the specification is configurable the resulting spec for using SVG instead is IVGS1_SA1_H1_I1_1(image_format: svg)

####Specification Example: 
 -A more constricted specification is needed than is inherent in the image so a new spec is registered and used for functionally constraining what image types can be used: IVGS1_SA1_H1_I1_1(image_format: IVGS1_I1_1)
  
