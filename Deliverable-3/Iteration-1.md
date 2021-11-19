# Iteration 1: Establishing an Overall System Structure

See: [System Requirements](https://github.com/icekoda/SD-FinalProject/blob/main/Deliverable-2/Deliverable-2.md#system-requirements)

## Step 2: Establish Iteration Goal by Selecting Drivers
We must observe the architectural convern CNR-1, whilst also considering all othe drivers, notably:
- UC-1 Add/Remove Items
- UC-2 Updating Items
- QA-2 Availability
- QA-3 Reliability
- QA-5 Maintainability
- CON-1 
- CON-2
## Step 4
| Design Decisions and Location   | Rationale |
| ----------- | ----------- |
|Logically Structure the client part as Rich Client Application reference architecture.|This reference architecture deals with an application that runs on the user’s machine. This directly supports CON-2, because the user can decide how to run the application, and has control over everything it does. It also satisfies CON-3, because this enables it to work without networking|

### Discarded Alternatives
| Alternative  | Reason |
| ----------- | ----------- |
|Web-Application|Contradicts CON-2, which requires the user being in control of the software. A web application would likely be managed by a third party.|

| Design Decisions and Location   | Rationale |
| ----------- | ----------- |
|Logically Structure the Server Structure using the Service Application reference architecture| By structuring the server as a Service Application, we can allow the service to run on the user’s machine, while the Client can access the service from the same device, or use multiple devices to access the same interface. This satisfies QA-1, QA-2, and CON-2.|
|Develop the Application with Ruby on Rails|We can utilize the ruby programming language, which we, the developers, are familiar with. Using this also benefits the user, as any updates can be made to the system while it is running. This satisfies QA-4, and QA-2|

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

| Design Decisions and Location   | Rationale |
| ----------- | ----------- |
|Store data on the main machine. If we have multiple machines, they can connect to the main machine, and any changes to the data are updated there.|This will ensure each machine is using data from the same location, and will ensure each machine is synchronized|

