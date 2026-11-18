# 29 - Electric Vehicle Inheritance

## Introduction
Specialized subclasses model domain-specific traits; an electric vehicle adds battery-specific fields and behavior on top of the base class.

## Scenario
Create an `ElectricVehicle` class deriving from `Vehicle` that adds battery capacity and charging time attributes, plus a method to estimate range based on capacity.

## Canonical Vehicle Attributes
The `ElectricVehicle` derived class adds the following private members (use these exact names and types):
- `double batteryCapacity` — battery capacity in kWh
- `float chargingTime` — hours to full charge

## Tasks to Implement
1. Create a derived class ElectricVehicle : public Vehicle.
2. Add batteryCapacity and chargingTime members.
3. Implement getter and setter methods.
4. Create displayElectricVehicleInfo(ElectricVehicle& ev).

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | ElectricVehicle ev("XYZ999","Tesla","Model 3",2023,15000.0f,true,'A',0.0); ev.setBatteryCapacity(75.0); ev.setChargingTime(8.5f); displayElectricVehicleInfo(ev); | Vehicle ID: XYZ999, Make: Tesla, Model: Model 3, Battery Capacity: 75, Charging Time: 8.5 |
| TC02 | ElectricVehicle ev("E1","Nissan","Leaf",2022,30000.0f,true,'A',0.0); ev.setBatteryCapacity(40.0); ev.setChargingTime(6.0f); displayElectricVehicleInfo(ev); | Vehicle ID: E1, Make: Nissan, Model: Leaf, Battery Capacity: 40, Charging Time: 6 |
| TC03 | ElectricVehicle ev("E2","Hyundai","Ioniq",2024,5000.0f,true,'A',0.0); ev.setBatteryCapacity(58.0); ev.setChargingTime(7.5f); displayElectricVehicleInfo(ev); | Vehicle ID: E2, Make: Hyundai, Model: Ioniq, Battery Capacity: 58, Charging Time: 7.5 |
| TC04 | ElectricVehicle ev("E3","MG","ZS EV",2023,18000.0f,true,'A',0.0); ev.setBatteryCapacity(50.0); ev.setChargingTime(8.0f); displayElectricVehicleInfo(ev); | Vehicle ID: E3, Make: MG, Model: ZS EV, Battery Capacity: 50, Charging Time: 8 |
| TC05 | ElectricVehicle ev("E4","BYD","Atto 3",2024,12000.0f,true,'A',0.0); ev.setBatteryCapacity(60.0); ev.setChargingTime(9.0f); displayElectricVehicleInfo(ev); | Vehicle ID: E4, Make: BYD, Model: Atto 3, Battery Capacity: 60, Charging Time: 9 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add `ElectricVehicle` derived class with `batteryCapacity` and `chargingTime`, implement required methods, and display results).
- A short `main()` or test harness that constructs `ElectricVehicle` objects, exercises the setters and display functions, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

