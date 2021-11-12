# Group 28 - Project Progress Report
## Business Case
With many people going hungry every day, food waste is a growing problem in our society. According to a 2019 report;
> In 2016, Canadians generated approximately 34 million tonnes of municipal solid waste.
> \- *Environment and Climate Change Canada*

Our goal is to make it easier to manage the food that you own, enabling you to purchase in bulk, and plan meals using software. In order to avoid food spoiling, we can use technology to help us organize our fridges, and freezers, allowing us to prepare meals based on shelf life.

## System Requirements
### Use Case Model
![Use Case](https://user-images.githubusercontent.com/73712369/140837370-446d2fef-1985-426d-8f49-492c80d60b8e.png)

| Use Case    | Description |
| ----------- | ----------- |
|UC-1 Add / Remove Items| Administrator is able to add any items wanted to the list at hand. They are also able to remove any item wanted from the list.|
|UC-2 Updating Items|Able to update the state of each item. Letting the user know each item's condition. Updates all connected systems update files.|
|UC-3 Search Inventory|Able to search an item by name or condition throughout the whole plate form. Able to see where the item is located, condition of the item, how many there are. |
|UC-4 Items List and State|Able to see the list of items and the condition the items are in. User must be able to sort food items based on expiration date, and must appear on home screen when expiration is imminent, or ocurring| 

### Quality Attribute Scenarios
| Attribute     | Description |
| ----------- | ----------- |
| QA-1 Performance      | Must be fast,intuitive, must be able to access all options in 3 clicks or less.       |
| QA-2 Availability  | Must be available 24 hours of the day. If over the network updates occur, it must do it live, with minimal downtime      |
| QA-3 Reliability | Must be able to sync with other systems, and database |
| QA-4 Maintainability    | Must have organized code that can be easily modified and reusable        |
| QA-5 User Friendly    | Must be easy to understand, easily accessible, easy to follow         |
| QA-6 Interoperability    | Must be able to interface with other smart home systems, to be easily integrated into a larger smart device ecosystem.        |
| QA-7 Accessibility    | Must be able to be installed with ease for enthusiasts, whether it be a tablet or raspberry pi.        |
### Constraints
1. The system must be able to run on hardware ranging in power, and monetary cost. Cheap in cost, and power. Should be able to run on a raspberry pi
2. Must follow open source model, must allow user to implement into their own applications or hardware.
3. Must be able to run with, or without networking.
