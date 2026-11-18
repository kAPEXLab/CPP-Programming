# 28 - Car Inheritance from Vehicle

## Introduction
Inheritance models real-world hierarchies and enables reuse. This task designs a `Car` derived class from a base `Vehicle`.

## Scenario
Extend `Vehicle` to create a `Car` class with car-specific attributes (like `numDoors` or `trunkCapacity`) and demonstrate using both base and derived class features.

## Canonical Vehicle Attributes
The `Car` derived class adds the following private members (use these exact names and types):
- `int numDoors` — number of doors
- `bool sunroof` — whether the car has a sunroof

## Tasks to Implement
1. Create a class Car : public Vehicle.
2. Add private members numDoors and sunroof.
3. Provide getter/setter methods for both.
4. Implement openSunroof(), closeSunroof(), lockDoors(), unlockDoors().
5. Create displayCarInfo(Car& car).

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Car c("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); c.setNumDoors(4); c.setSunroof(true); displayCarInfo(c); | Vehicle ID: ABC123, Make: Toyota, Model: Camry, Year: 2022, Doors: 4, Sunroof: 1 |
| TC02 | Car c("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); c.setNumDoors(4); c.setSunroof(false); displayCarInfo(c); | Vehicle ID: XYZ999, Make: Honda, Model: Civic, Year: 2021, Doors: 4, Sunroof: 0 |
| TC03 | Car c("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); c.setNumDoors(5); c.setSunroof(true); displayCarInfo(c); | Vehicle ID: BMW77, Make: BMW, Model: X5, Year: 2020, Doors: 5, Sunroof: 1 |
| TC04 | Car c("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); c.setNumDoors(5); c.setSunroof(true); displayCarInfo(c); | Vehicle ID: TESLA7, Make: Tesla, Model: Model Y, Year: 2024, Doors: 5, Sunroof: 1 |
| TC05 | Car c("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); c.setNumDoors(4); c.setSunroof(false); displayCarInfo(c); | Vehicle ID: AUDI08, Make: Audi, Model: A4, Year: 2019, Doors: 4, Sunroof: 0 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add `Car` derived class with `numDoors` and `sunroof`, implement required methods, and display results).
- A short `main()` or test harness that constructs `Car` objects, exercises the setters and display functions, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

