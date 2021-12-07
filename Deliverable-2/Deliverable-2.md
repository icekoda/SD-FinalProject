# Group 28 - Project Progress Report
## Business Case
With many people going hungry every day, food waste is a growing problem in our society. According to a 2019 report;
> In 2016, Canadians generated approximately 34 million tonnes of municipal solid waste.
> \- *Environment and Climate Change Canada*

Our goal is to make it easier to manage the food that you own, enabling you to purchase in bulk, and plan meals using software. In order to avoid food spoiling, we can use technology to help us organize our fridges, and freezers, allowing us to prepare meals based on shelf life.

## System Requirements
### Use Case Model
![Use Case](https://user-images.githubusercontent.com/73712369/140837370-446d2fef-1985-426d-8f49-492c80d60b8e.png)

These use cases can be described in the following table.

| Use Case    | Description |
| ----------- | ----------- |
|UC-1 Add, Remove, Update Items| Administrator is able to add any items wanted to the list at hand. They are also able to remove any item wanted from the list.|
|UC-2 Login   | Have a login page, where users with different privileges can sign in|
|UC-3 Register| Allow users to create an account|
|UC-4 Search Inventory|Able to search an item by name or condition throughout the whole plate form. Able to see where the item is located, condition of the item, how many there are. |
|UC-5 Manage User Permissions| Allow the modification of permissions for each user.|
|UC-6 Highlight Items of Interest| Front page of interface will highlight and show items of interest, such as expiring within the next week, or based on time of year, such as showing Christmas decorations at Christmas.|
|UC-7 Items List and State|Able to see the list of items and the condition the items are in. User must be able to sort food items based on expiration date, and must appear on home screen when expiration is imminent, or ocurring| 
|UC-8 Item Ownership | Allow ownership of items to be specified, to clairify privileges when interacting with items|

### Quality Attribute Scenarios
In addition to the stated use cases, some quality attributes were then documented. We also connect their
| Attribute     | Scenario | Associated Use Case |
| ----------- | ----------- | ----------- |
| QA-1 Performance      | Must be fast,intuitive, must be able to access all options in 3 clicks or less.       | ALL |
| QA-2 Availability  | Must be available 24 hours of the day. If over the network updates occur, it must do it live, with minimal downtime | ALL|
| QA-3 Reliability | Must be able to sync with other systems, and database | UC-1, UC-4|
| QA-4 Maintainability    | Must have organized code that can be easily modified and reusable | 
| QA-5 User Friendly    | Must be easy to understand, easily accessible, easy to follow| ALL|
| QA-6 Interoperability    | Must be able to interface with other smart home systems, to be easily integrated into a larger smart device ecosystem.| UC-1, UC-4|
| QA-7 Accessibility    | Must be able to be installed with ease for enthusiasts, whether it be a tablet or raspberry pi. Open Source model.|
| QA-8 Security | Must have passwords be stored as hash to protect passwords.| UC-2, UC-3 |
### Constraints - *CON*
| Constraint     | Description | Associated Quality Attribute |
| ----------- | ----------- |  ----------- |
| CON-1       | User can connect to local server running the application through web browser over a slow connection. | QA-2 |
| CON-2       | Entire user interface must be accessed through web browser | QA-5
| CON-3       | All system events within past 10 days must be logged | QA-4 |
| CON-4       | A backend relational database server must be utilized | QA-7, QA-2 |
| CON-5       | Application must be able to run on low end hardware, such as Raspberry Pi | QA-1, QA-7 |
