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
|Website Interface                | Will be able to interact with both the user and application created. It is able to display results from requests.

## Step 6: Sketch Views and Record Design Decisions
| Element                         |            Responsibility |
| -----------                     |               ----------- |
| DisplayList                     | When called, fetches list and displays it | 
| DatabaseConnector               | Responsible for interacting with the database, performing SQL queries, and passing information through|
| ItemController                  | Responsible for facilitating interactions with the items. |
| UserService                     | Receives requests from the user |



