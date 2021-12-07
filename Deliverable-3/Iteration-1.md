# Iteration 1: Establishing an Overall System Structure

See: [System Requirements](https://github.com/icekoda/SD-FinalProject/blob/main/Deliverable-2/Deliverable-2.md#system-requirements)

## Step 2: Establish Iteration Goal by Selecting Drivers
We must keep in mind all the drivers that influence the general structure of the system, but we notably observe the drivers in the following table
| Driver  | Description |
| ----------- | ----------- |
| QA-1 | Peformance|
| QA-2 | Availability|
| QA-6 | Interoperability |
| CON-1 | User can connect to local server running the application through web browser over a slow connection.|
| CON-4 | A backend relational database server must be utilized|
| CON-5 | Application must be able to run on low end hardware, such as Raspberry Pi|

## Step 3: Choose One or More Elements of the System to Refine
We are going to refine the entire system.
## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers 
| Design Decisions and Location   | Rationale |
| ----------- | ----------- |
|Logically structure the client part of the system as **Web Application** reference architecture|This reference architecture deals with an application that is interfaced directly through the web browser. This directly supports CON-1, because the user can acccess the application on multiple devices with the same interface. It can also support QA-6, as it is interoperable with any device capable of running a modern web browser.|
| Logically structure the server partition of the system as a **Service Application** | This structure will allow a unified envrionment for multiple instances accessing the application. This coincides with QA-2, as well as QA-6. This also supports CON-5 and CON-4 because the user can decide where to run the application, and has control over everything it does. |
| Three-Tier Deployment Pattern | We will use a three-tier deployment to support the project consisting of a server backend, database, and client web application |

### Discarded Alternatives
| Alternative  | Reason |
| ----------- | ----------- |
|Rich Client|Does not support QA-2 as it would only be available on one system.|
|Mobile Application | Does not support QA-2, QA-6, CON-4, as it also not be able to run on more than one system|

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

| Design Decisions and Location   | Rationale |
| ----------- | ----------- |
| Store logging data on the main server. If we have multiple machines, they can connect to the main machine, and any changes to the data are updated there.|This will ensure each machine is using data from the same location, and will ensure each machine is synchronized |
| Allow utilizing of third database server | Can allow more storage or different storage locations |

## Step 6: Sketch Views and Record Design Decisions
| Element   | Rationale |
| ----------- | ----------- |
| Client      | Hosts client side logic and user interactions |
| Server      | Runs the main application. Coordinates web pages, and all server logic |
| DataBase Server | Hosts the main database, can run on same machine as main server, or external database |

![Architecture](https://user-images.githubusercontent.com/73712369/144958994-f9dd84ac-7c59-4c98-bc8d-59246084701e.png)
![Layers](https://user-images.githubusercontent.com/73712369/144959322-f34abccb-06bd-49ec-a111-7b7de59b602f.png)



