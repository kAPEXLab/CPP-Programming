# 32 - Fuel Efficiency Polymorphism

## Introduction
Polymorphism allows calling derived implementations through a base pointer or reference. This enables different efficiency calculations for different vehicle types.

## Scenario
Define a virtual `calculateEfficiency()` method in `Vehicle` and override it in derived classes (`Car`, `ElectricVehicle`, etc.) to compute fuel or energy efficiency polymorphically.

## Tasks to Implement
1. Create a Vehicle class with calculateFuelEfficiency().
2. Create Car and Truck classes with overridden implementations.
3. Implement a template function compareFuelEfficiency(Vehicle& vehicle1, Vehicle& vehicle2).
4. Display which vehicle has better fuel efficiency.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Car c("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Truck t("DEF456","Ford","Transit",2021,70000.0f,false,'M',3.5); compareFuelEfficiency(c, t); | The vehicle with higher fuel efficiency is reported. |
| TC02 | Car c("V1","Honda","Civic",2021,45000.0f,false,'A',1.8); Truck t("V2","Tesla","Semi",2024,5000.0f,true,'A',0.0); compareFuelEfficiency(c, t); | The vehicle with higher fuel efficiency is reported. |
| TC03 | Car c("B1","BMW","X5",2020,68000.0f,false,'A',3.0); Truck t("B2","Ford","Transit",2021,70000.0f,false,'M',3.5); compareFuelEfficiency(c, t); | The vehicle with higher fuel efficiency is reported. |
| TC04 | Car c("T1","Toyota","Fortuner",2022,32000.0f,false,'A',2.8); Truck t("T2","Mahindra","BOLERO",2021,61000.0f,false,'M',1.9); compareFuelEfficiency(c, t); | The vehicle with higher fuel efficiency is reported. |
| TC05 | Car c("A1","Audi","A4",2019,74000.0f,false,'M',2.0); Truck t("A2","Mercedes","Sprinter",2022,53000.0f,false,'M',2.1); compareFuelEfficiency(c, t); | The vehicle with higher fuel efficiency is reported. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add virtual `calculateFuelEfficiency()` to `Vehicle`, override in derived classes, and implement the comparison function).
- A short `main()` or test harness that constructs the sample vehicles and calls `compareFuelEfficiency()` to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

