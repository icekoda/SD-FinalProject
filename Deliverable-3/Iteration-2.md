Previous: [Iteration-1](https://github.com/icekoda/SD-FinalProject/blob/main/Deliverable-3/Iteration-1.md)

Next: [Iteration-3](https://github.com/icekoda/SD-FinalProject/blob/main/Deliverable-3/Iteration-3.md)
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
| Use Case   | Description |
| -----------                     |               ----------- |
| UC-1 | Add, Remove, Update Items |
| UC-2 | Login |
| UC-3 | Register |
| UC-4 | Search Inventory |

## Step 3: Choose One or More Elements of the System to Refine 
The elements that are being refined are modules that support core functionality.
## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Create a Domain model            | It is important to define conceptsand how they are related in the functionality of the application.|
| Create Domain Objects           | Each element of the application needs to be defined as a domain object |


## Step 5: Instantiate Architectural  Elements, Allocate  Responsibilities, and Define Interfaces 
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Create only an initial Domain model       | We need to describe the entities that participate in the primary use case.|
|Map the system use cases to domain objects| Objects must be identified for all the use cases|


## Step 6: Sketch Views and Record Design Decisions
| Element                         |            Responsibility |
| -----------                     |               ----------- |
| Account                   | Manages user accounts and their information | 
| Client               | Responsible for interacting with the application server.|
| IventoryManagerDBMS                  | Main application server. |
| Inventory Database                   | Stores all data for each item |
| Item               | Contains information about each item |

##### Figure 1: Domain Model
![Management_inventory_Use_case drawio1](https://user-images.githubusercontent.com/73712369/144962610-09817c08-8978-4346-97d1-1f8164f84acc.png)

##### Figure 2: Package Diagram
![Management_inventory_Use_case drawio](https://user-images.githubusercontent.com/73712369/144962870-e0457e2a-4e10-4d2d-8b15-c9cc3e97b0a8.png)


##### Figure 3: Sequence Diagram For UC-1
![Inventory_Manger_Sequence_Diagram](https://user-images.githubusercontent.com/73712369/144963889-43155bda-e77f-482c-9f8a-c8927d0e4bb1.png)


