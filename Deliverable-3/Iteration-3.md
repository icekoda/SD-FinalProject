Previous: [Iteration-2](https://github.com/icekoda/SD-FinalProject/blob/main/Deliverable-3/Iteration-2.md)

# Iteration 3: Addressing  Quality Attribute Scenario Driver
Building on the fundamental structural decisions made in iteration 1 & 2, we can now focus on the fulfilment of a quality attribute. This iteration focuses on just one quality attribute

## Step 2: Establish Iteration Goal by Selecting Drivers 
For this iteration the architect focuses on the QA-8 quality attribute scenario:
Must have passwords be stored as hash to protect passwords.

## Step 3: Choose One or More Elements of the System to Refine
We will refine component:
**Account**

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers 
| Design Decisions and Location   | Rationale and Assumptions |
| -----------                     |               ----------- |
|Introduce a password hasher | By implementing this element, we can safely store passwords in the local storage, as to ensure they are safely kept secret in case of a data breach|
|Introduce an element that can manage logins, and check hashes| This will manage user logins |

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
| Element                         | Responsibility             |
| -----------                     |               ----------- |
| PasswordHasher                  | This element will take in password inputs, and then hash them, and pass them along|
| HashChecker                  | This will check the inputed hash with the hash stored on file, and return whether they match|

## Step 6: Sketch Views and Record Design Decisions 
![Layewr_Inventory_ drawio_1](https://user-images.githubusercontent.com/73712369/144965391-6019ed2f-0996-4a67-88f6-c34d0a595f62.png)
