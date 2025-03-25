[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/rXX1_Uiw)
## Project 00
### NeXTCS
### Period: 9
## Name0: Juliet Badillo Flores
## Name1: Angela Yee
---

This project will be completed in phases. The first phase will be to work on this document. Use github-flavoured markdown. (For more markdown help [click here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) or [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) )

All projects will require the following:
- Researching new forces to implement.
- Method for each new force, returning a `PVector`  -- similar to `getGravity` and `getSpring` (using whatever parameters are necessary).
- A distinct demonstration for each individual force (including gravity and the spring force).
- A visual menu at the top providing information about which simulation is currently active and indicating whether movement is on or off.
- The ability to toggle movement on/off
- The ability to toggle bouncing on/off
- The user should be able to switch _between_ simluations using the number keys as follows:
  - `1`: Gravity
  - `2`: Spring Force
  - `3`: Drag
  - `4`: Custom Force
  - `5`: Combination


## Phase 0: Force Selection, Analysis & Plan
---------- 

#### Custom Force: Repulsion

### Forumla
What is the formula for your force? Including descriptions/definitions for the symbols. (You may include a picture of the formula if it is not easily typed.)

![image](https://github.com/user-attachments/assets/3cea99a8-108a-45ee-b716-68987045c927)


### Custom Force
- What information that is already present in the `Orb` or `OrbNode` classes does this force use?
  - it is similar to gravity formula. so it will use distance squared.

- Does this force require any new constants, if so what are they and what values will you try initially?
  - k = 8.988 * 10^9 (N*m^2)/c^2

- Does this force require any new information to be added to the `Orb` class? If so, what is it and what data type will you use?
  - sign classifcation

- Does this force interact with other `Orbs`, or is it applied based on the environment?
  - based on other orbs

- In order to calculate this force, do you need to perform extra intermediary calculations? If so, what?
  - erm maybeee idk

--- 
### Simulation 1: Gravity
Describe how you will attempt to simulate orbital motion.
![image](https://github.com/user-attachments/assets/5030223c-a0f3-4b00-8036-c745d859c7ab)


--- 

### Simulation 2: Spring
Describe what your spring simulation will look like. Explain how it will be setup, and how it should behave while running.

At set length, it will turn red when stretched and green when compressed from the center of the orbs.

--- 

### Simulation 3: Drag
Describe what your drag simulation will look like. Explain how it will be setup, and how it should behave while running.


![image](https://github.com/user-attachments/assets/cf7e3aca-274f-42f2-ab79-136b79892d89)


--- 

### Simulation 4: REPSULSION
Describe what your Custom force simulation will look like. Explain how it will be setup, and how it should behave while running.

Will cause orbs to repel each other. Depends based on opposite charges and magnitude of charges (maybe can identify + or - charges with color?) Assign orbs a number 1 or 2. If orb = 1, it will be negative. If orb = 2, it will be positive. Move orb together or apart a certain distance based on the charges and multiply them by their mass and constant.

--- 

### Simulation 5: Combination
Describe what your combination simulation will look like. Explain how it will be setup, and how it should behave while running.

Huge mess!!!
The fixed orb will attract the other orbs due to gravity. The Orbs are attached by springs. They will also repel and deviate from the "natural order" they are in bc of their charges. This will affects the other orbs bc of drag force. Their movements will also undergo collsions and chaos. 

