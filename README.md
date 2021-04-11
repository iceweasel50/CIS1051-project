# Proposal

## What will (likely) be the title of your project?

Battery Management system

## In just a sentence or two, summarize your project. (E.g., "A website that lets you buy and sell stocks.")

arduino that takes in voltage and current in a battery and determines if it should open a switch or not to save the life of the battery 

## In a paragraph or more, detail your project. What will your software do? What features will it have? How will it be executed?

The software will read the voltage and current from the battery. it will determine the state of charge (SOC). Then detremine if the soc is below a certian threshold for a specified amount of time. If the voltage meets the criteria the arduino will actuate a servo to open a switch.  

## If planning to combine 1051's final project with another course's final project, with which other course? And which aspect(s) of your proposed project would relate to 1051, and which aspect(s) would relate to the other course?

This is a project that I have been working on for my engineering Capstone class. The coding part will relate to 1051 and the mechanical and design part of it will relate to the engineeering class. 

## If planning to collaborate with 1 or 2 classmates for the final project, list their names, email addresses, and the names of their assigned TAs below.

TODO, if applicable

## In the world of software, most everything takes longer to implement than you expect. And so it's not uncommon to accomplish less in a fixed amount of time than you hope.

### In a sentence (or list of features), define a GOOD outcome for your final project. I.e., what WILL you accomplish no matter what?

After the final phase of the project, the Battery Management System will be able to detect a vehicle's battery voltage and determine if it will be able to successfully start. If it is determined that the voltage will not suffice for a full vehicle start, then the power to vehicle will be terminated, saving the battery from full depletion. 

### In a sentence (or list of features), define a BETTER outcome for your final project. I.e., what do you THINK you can accomplish before the final project's deadline?

Realistically speaking I would like to have the Battery Monitoring System possess the capability to do the above as well as deterime a battery's state of charge (SOC). This would set the "cut off" threshold dynamically based on the specific battery / vehicle. 

### In a sentence (or list of features), define a BEST outcome for your final project. I.e., what do you HOPE to accomplish before the final project's deadline?

In a perfect world I would have the all of the above as well as having a way to automate the state (on or off) of the arduino itself. Although the Battery Monitoring System would still be fairly functional without this feature, having it would allow for a "deploy and forget" method to the unit.  


## In a paragraph or more, outline your next steps. What new skills will you need to acquire? What topics will you need to research? If working with one of two classmates, who will do what?

I will have to brush up on C programming. I will have to reserch more into how batteries work. Additionally I will have to understand the math equations that realte the current and the voltage to determine the state of charge. 

