# 30 - Electric Car Multiple Inheritance

## Introduction
Multiple inheritance lets a class combine features from more than one base; use it carefully to avoid ambiguity. This task explores mixing vehicle traits.

## Scenario
Design an `ElectricCar` that inherits from `Car` and an `Electric` interface/class (e.g., `BatterySpecs`) to combine typical car features with electric-specific behavior like `charge()`.

## Canonical Vehicle Attributes
The `ElectricCar` combines car and EV attributes — include only the additional members required by this task (use these exact names and types):
- `int numDoors` — number of doors (from `Car`)
- `bool sunroof` — whether the car has a sunroof (from `Car`, optional)
- `double batteryCapacity` — battery capacity in kWh (from `ElectricVehicle`)

## Tasks to Implement
1. Create a class ElectricCar : public Car, public ElectricVehicle.
2. Implement displayElectricCarInfo().
3. Display vehicle details, car-specific details, and EV-specific details.
4. Validate the printed output.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | ElectricCar ec("XYZ999","Tesla","Model S",2022,20000.0f,true,'A',0.0); ec.setNumDoors(4); ec.setBatteryCapacity(100.0); ec.displayElectricCarInfo(); | Vehicle ID: XYZ999, Make: Tesla, Model: Model S, Doors: 4, Battery Capacity: 100 |
| TC02 | ElectricCar ec("E1","Nissan","Leaf",2022,35000.0f,true,'A',0.0); ec.setNumDoors(4); ec.setBatteryCapacity(40.0); ec.displayElectricCarInfo(); | Vehicle ID: E1, Make: Nissan, Model: Leaf, Doors: 4, Battery Capacity: 40 |
| TC03 | ElectricCar ec("E2","Hyundai","Ioniq",2024,5000.0f,true,'A',0.0); ec.setNumDoors(4); ec.setBatteryCapacity(58.0); ec.displayElectricCarInfo(); | Vehicle ID: E2, Make: Hyundai, Model: Ioniq, Doors: 4, Battery Capacity: 58 |
| TC04 | ElectricCar ec("E3","MG","ZS EV",2023,18000.0f,true,'A',0.0); ec.setNumDoors(5); ec.setBatteryCapacity(50.0); ec.displayElectricCarInfo(); | Vehicle ID: E3, Make: MG, Model: ZS EV, Doors: 5, Battery Capacity: 50 |
| TC05 | ElectricCar ec("E4","BYD","Atto 3",2024,12000.0f,true,'A',0.0); ec.setNumDoors(5); ec.setBatteryCapacity(60.0); ec.displayElectricCarInfo(); | Vehicle ID: E4, Make: BYD, Model: Atto 3, Doors: 5, Battery Capacity: 60 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement `ElectricCar` multiple inheritance, display method, and demonstrate it).
- A short `main()` or test harness that constructs `ElectricCar` objects, sets required fields, calls `displayElectricCarInfo()`, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

