# Iteration 3: Addressing  Quality Attribute Scenario Driver
Building on the fundamental structural decisions made in iteration 1 & 2, we can now focus on the fulfilment of a quality attribute. This iteration focuses on just one quality attribute

## Step 2: Establish Iteration Goal by Selecting Drivers 
For this iteration the architect focuses on the QA-2 quality attribute scenario:
The system must be available 24/7, and must make sure server is running before executing any queries

## Step 3: Choose One or More Elements of the System to Refine
We will refine component:
NetworkManager

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers 
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Introduce the Detect Faults tactic | By implementing this element, the system can withstand network interruptions|

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
| Element                         | Responsibility             |
| -----------                     |               ----------- |
| NetworkManager                  | By implementing this element, the system can withstand network interruptions|
| Heartbeat                       | Pings database, and application server, and returns a value depending on if it's available

![Sequence_Diagram_2](https://user-images.githubusercontent.com/73712369/142655139-24b530dd-48e1-46dd-a953-4a6f3e626684.png)

## Step 6: Sketch Views and Record Design Decisions 
![Sequence_Diagram_2](https://user-images.githubusercontent.com/73712369/142656996-4d5ade17-0852-4dcb-aadf-13f32496b042.png)
