# Iteration 2 - Identifying Structures to Support Primary Functionality 

This section presents the results of the activities that are performed in each of the steps
of ADD in the second iteration of the design process for the FCAPS system. We move from the generic and
coarse-grained descriptions of functionality used in iteration 1 to more detailed
decisions that will drive imple-mentation and hence the formation of development teams 

## Goal

> Reason about the units of implementation, which affect team formation, interfaces, and the means by
  which development tasks may be distributed, outsourced, and implemented in sprints.
  
## Step 2: Establish Iteration Goal by Selecting Drivers
The goal of this iteration is  to address the general architectural concern of identifying structures
to support primary functionality. In the second iteration, the architect considers the system's primary
use cases:
- UC-1
- UC-3

## Step 3: Choose One or More Elements of the System to Refine 
The elements that are being refined are modules that support core functionality.
## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Create a Domain model            | It is important to define conceptsand how they are related in the functionality of the application.
| 

## Step 5: Instantiate Architectural  Elements, Allocate  Responsibilities, 
and Define Interfaces 
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Create only a Domain model       | We need to describe the entities that participate in the primary use case.|
|Map the system use cases to domain objects| Objects must be identified for all the use cases|


## Step 6: Sketch Views and Record Design Decisions
| Element                         |            Responsibility |
| -----------                     |               ----------- |
| DisplayList                     | When called, fetches list and displays it | 
| DatabaseConnector               | Responsible for interacting with the database, performing SQL queries, and passing information through|
| ItemController                  | Responsible for facilitating interactions with the items. |
| UserService                     | Receives requests from the user |
| ViewController                  | Controls and update views. When user interacts with the system, it checks the view controller for any updates |

##### Figure 1: Domain Model
![Management_inventory_Use_case drawio1](https://user-images.githubusercontent.com/73712369/142634792-56ffee30-0440-44a2-8615-75098b371f11.png)

##### Figure 2: Domain objects
![Management_inventory_Use_case drawio](https://user-images.githubusercontent.com/73712369/142634811-1d4594fc-f68d-424f-bbba-4b66bea240d5.png)

##### Figure 3: Sequence Diagram For UC-1
![Inventory_Manger_Sequence_Diagram](https://user-images.githubusercontent.com/73712369/142639791-6cf6db3c-d93c-48e2-bd3b-69434cdee785.png)

## Step 7: Perform Analysis of Current Design and Review Iteration Goal and Achievment of Design Purpose


