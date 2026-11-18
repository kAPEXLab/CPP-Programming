# 36 - Engine Composition

## Introduction
Composition models 'has-a' relationships: vehicles have engines. This allows separating engine details into a dedicated class.

## Scenario
Implement an `Engine` class and include it as a member of `Vehicle`. Provide methods that delegate to engine behavior (e.g., `getHorsepower()`) and demonstrate composition.
## Canonical Vehicle Attributes

This scenario requires an `Engine` class with the following members (use these exact names and types):
- `std::string engineType`
- `int horsepower`
- `int torque`

Also add an `Engine engine` member to `Vehicle` and provide accessor/mutator methods as required.

## Tasks to Implement
1. Create an Engine class with engineType, horsepower, and torque.
2. Add an Engine member to Vehicle.
3. Modify displayVehicleInfo() to print engine details.
4. Create a sample vehicle with a custom engine.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); v.setEngine("Hybrid",180,220); v.displayVehicleInfo(); | Engine Type: Hybrid, Horsepower: 180, Torque: 220 |
| TC02 | Vehicle v("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); v.setEngine("Petrol",140,180); v.displayVehicleInfo(); | Engine Type: Petrol, Horsepower: 140, Torque: 180 |
| TC03 | Vehicle v("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); v.setEngine("Diesel",210,320); v.displayVehicleInfo(); | Engine Type: Diesel, Horsepower: 210, Torque: 320 |
| TC04 | Vehicle v("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); v.setEngine("Electric",320,500); v.displayVehicleInfo(); | Engine Type: Electric, Horsepower: 320, Torque: 500 |
| TC05 | Vehicle v("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); v.setEngine("Turbo",190,260); v.displayVehicleInfo(); | Engine Type: Turbo, Horsepower: 190, Torque: 260 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add `Engine` class, include as a member in `Vehicle`, expose accessors, and display engine details).
- An `Engine` class with the following public API:
	- `Engine();`
	- `Engine(const std::string& engineType, int horsepower, int torque);`
	- `std::string getEngineType() const;` / `void setEngineType(const std::string&);`
	- `int getHorsepower() const;` / `void setHorsepower(int);`
	- `int getTorque() const;` / `void setTorque(int);`
- `Vehicle` additions required by this question (only these):
	- `void setEngine(const std::string& engineType, int horsepower, int torque);`
	- `Engine getEngine() const;`
	- `void displayVehicleInfo() const;` (must print engine details as part of vehicle info)
- A short `main()` or test harness that constructs vehicles, sets engine details via `setEngine(...)` or `Engine` constructor, calls `displayVehicleInfo()`, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

