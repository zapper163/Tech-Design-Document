# TECH DESIGN DOCUMENT (TDD)

## Introduction
The Technical Design Document provides a blueprint for the software engineers in your team to implement and code the features of your game. The technical design document will let your developers to specify - what are the requirements, how they should be implemented, along with the tools and technologies required for the implementation. The connection between structural design of a Software and Technical Design Document is that the technical design document has a broader scope with less details, than a software architecture diagram.

The primary function of a TDD is to communicate the technical details of the work to be done to members of the team. However, there is a second purpose which is just as important: the process of writing the TDD forces you to organize your thoughts and consider every aspect of the design, ensuring that you haven’t left anything out.

This process is highly variable; the set of steps listed here will change on a case-by-case basis. For example:
For smaller features that don’t involve a lot of complexity, steps 2 and 3 will often be combined into a single document.
If the feature involves a large number of unknowns or some level of research, it may be necessary to construct a proof-of-concept implementation before finalizing the technical design.

This process also happens at different scales and levels of granularity. A PRD / TRD / TDD may concern the design of an entire system, or just a single feature. In most environments, the process is also cyclic — each design/implement cycle builds on the work of the previous one.

## Content

A TDD generally contains the following information:

- List of all features.
- Choice of Game engine
- High level diagrams
- Details about the 3D objects, terrain, scenes.
- Use of Physics Engine
- Game logic and artificial intelligence
- Audio and Visual details and specifications
- Networking
- Delivery platform & hardware/software requirements for running the game on a system.

[Source](https://www.studytonight.com/3d-game-engineering-with-unity/tdd-and-gdd)

[Source](https://medium.com/machine-words/writing-technical-design-docs-71f446e42f2e)


## TDD Template

### Technical goals
The technical goals are a list of objectives set to ensure everyone inside the team knows where to aim when working. They define what is expected to achieve in relation to the code, the game engine or the platform where the game is going to be delivered. Some examples would be immersive ambient sound, complex AI or realistic shadows.

### Technical risks
At the same time a team has its goals there are also risks which must not be overlooked. If the game has a level with a large map like in any Hitman game, one of those risks could be that the fact of having a vast number of entities and NPC's loaded at the same time makes the game go incredibly slow. In order to take the risks into account they are written down in the TDD.


### Code style guidelines
Being one of the most important of the TDD, in this section are described the code conventions that will be applied during the development of the whole project, in order to have an organized and homogeneous code that every programmer of the team is able both to understand and to work with. The thoroughness of the code style guidelines depends on the programming team and their objectives. Here are some examples of the elements one could find in this section:

 - **Naming rules:** Explains in which language the code must be, how variables and functions must be named, the use of signs like parentheses and whitespaces or the need of     using comments. For example:

  Every #define must be in capital letters:
  #define MAX_HP 300
  
 - **Variables:** Explains how to manage the variables, how to declare and initialize them and whether to declare them inside public, protected or private part when using        classes or structs. For example:

  Every time a pointer is created must be initialized as null:
  int* test = nullptr;
  
 - **Loops:** Mentions which loops are preferred inside the code (while, do-while, for…) and when to use break and continue keywords.

 - **Conditionals:** Describes how to manage conditionals, whether to separate the if line from the functions inside the conditional or to put everything in the same line, when  to use scopes {} or if it is preferred a conditional with operators or without them. For example:

  We prefer a conditional like if(something) {}
  rather than one like if(something == true) {}
  
 - **Classes & structs:** It is basically a convention of when to use classes and when structs and how to write the elements inside them.

 - **XML:** Outlines the guidelines to write the variables in the XML files of the project and how to name their nodes and attributes. For example:

 If a node has just one attribute we'll declare it in the same line:
 <house colour="red"/>
 
### External libraries
In this section are detailed the external libraries which are going to be used for the development of the project and what are they going to be used for.

### Code organization overview 
Offers a general outlook of the structure the code will have and the inheritance relation between its classes. These diagrams show the functions and the variables included in each module. It is a guide used to see the whole picture of the code. Nevertheless, this guide will change as the project goes by and the game evolves, becoming more complex each time and being extended with more specified UML diagrams of the emergent code modules.

### Performance budgets
Related with the technical goals, the performance budgets are a series of limits imposed on the metrics that affect the game performance. Those could be the frames per second the game runs, the amount of disk memory is occupied by a certain feature of the game or the time it is expected for a map to be loading. Performance budgets serve as a point of reference for making decisions about design, technology and adding features. That enables the team to approach to the game with an established mentality about which standards their final result must accomplish.


### Build delivery method
This section describes the process that will be followed every time a build is delivered. It explains if there will be used an extern program, who will deliver the build and when will it be delivered.

### Version list
Planning beforehand what it is intended to have for each version of the game creates a guideline to follow when it comes to create the releases. In this way the team can identify in which phase of the development they are. 

### Delivery platform and requirements
It defines the target platform for which the game will be delivered, such as PC, Xbox, PS4 or other consoles. In addition, in this section is specified the minimum and the recommended hardware and software which are required to play it.

## Extra sections
The extra sections of a TDD are those which vary depending on the game or are not as important or necessary as the core sections.

### Choice of game engine
If the game is going to use a game engine this section explains which one has been decided to use and the reasons of this election. It also has a brief description of the features the chosen engine provides to the developers.

### Art and audio tools
In case there is no Art Bible and no Audio Bible, this section will specify which art tools will be used for the game art and audio and which tool will be used for each art or audio area.

### 3D Objects, terrain and scene management
In this section is explained which objects will be in each part of the map, which terrains will be used in the game and how will be the scene management.

### Use of physics engine
This section describes how will be de collision detection, how will be the physics calculated and applied to the game (gravity, friction…) and how will be the interaction of the characters or the other entities with the game world.

### Artificial Intelligence
If the game will have a complex AI system, it is very important it is conscientiously planned and detailed.

### Networking
In the case the game is multiplayer or has a multiplayer mode this section explains how it will be handled.


## Sources:
- [Source](https://www.studytonight.com/3d-game-engineering-with-unity/tdd-and-gdd)

- [Source](https://medium.com/machine-words/writing-technical-design-docs-71f446e42f2e)

- [How to write a better technical design document](https://www.range.co/blog/better-tech-specs)

- [How to write technical design docs](https://dev.to/mage_ai/how-to-write-technical-design-docs-c02)














### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
