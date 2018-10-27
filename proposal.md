# X-Team n/a Kitchen Tasks by Priority Proposal

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

I work as a kitchen manager in a restaurant with many dishes. These dishes all require different ingredients and procedures that vary in both time and difficulty.  

I want to create a priority queue that will be able to sort through patrons' orders and let the chefs know what tasks they should be focusing on in order to get every dish out in a timely, efficient manner. For example, one customer may order a pasta dish, while another orders a salad. It would be inefficent to waste time while the noodles are boiling, so seperate tasks should be assigned after the noodles are put to boil (e.g. chopping vegetables for the salad). Each task should be associated with the time it takes to perform, as well as the dish that requires it.  

The program should have a Main.java file that will record what dishes are ordered, also handling input and output. 

The program should implement a priority queue in order to assign the order that tasks ought to be completed in.  

Ample testing should be done in order to determine that dishes are still being prepared correctly.


## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)

Proposal name: Kitchen Tasks by Priority.


2. Output: Describe the output your program will produce.  Include an example format of the output produced.

The program will output a dynamic listing of kitchen tasks that should be done, ordered by highest priority and time required.
High priority will be determined by tasks that need to be completed before others (e.g. chopping vegetables is prioritized before tossing the salad). When the time associated with a priority has elapsed (# minutes - 1), the priority is reset. The program will output that a dish is ready for serving if all associated tasks have been completed. 

*Example:*  
* Task 1: Boil spaghetti noodles (Spaghetti; Priority: 1, 6 minutes)  
* Task 2: Chop carrots (Salad; Priority: 2, 1 minute)  
* Task 3: Chop lettuce (Salad; Priority: 2, 1 minute)  
* Task 4: Chop cucumbers (Salad; Priority: 2, 1 minute)  
* Task 4: Make salad dressing (Salad; Priority: 2, 2 minutes)  
* Task 5: Remove noodles from water (Spaghetti; Priority: 1, 1 minute)  
* Task 6: Saute noodles (Spaghetti; Priority: 1, 4 minutes)  
* Task 7: Toss Salad (Salal; Priority: 2, 2 minutes)  
* *Salad is ready for serving*  
* *Spaghetti is ready for serving*  


3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

The input required is simply the dishes that have been requested, in the correct order. The program will implement a class that has all data related to cooking tasks readily available.  

*Example:*  
* House Salad  
* Spaghetti with meat sauce  


4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

The user interface will be relatively simple, a text menu that will allow the user to enter dishes ordered, and also see all the current tasks.


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.

##TODO


Name each interface or class and briefly describe its function or purpose.

* KitchenPriorityQueue - this queue will store the input and output the tasks by priority.  
* CookingTasks - this class has all data related to cooking tasks associated with the dishes at this restaurant.


## Edit and Submit this file and any figures referenced by this document.

