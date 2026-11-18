# 02 - Setter Methods for Vehicle Properties

## Introduction
Maintaining consistent and validated updates to vehicle attributes is crucial. This task emphasizes creating setter methods that validate inputs and update internal state safely.

## Scenario
In a vehicle inventory tool, users will update vehicle attributes after inspections or repairs. Implement setter methods that enforce simple validation rules (non-empty strings, reasonable year and mileage ranges) and update the object's state accordingly.

## Canonical Vehicle Attributes
No new attributes are required in this question; use the base `Vehicle` members introduced earlier.

## Tasks to Implement
1. Implement setter methods for each property in the Vehicle class.
2. Keep each method focused on a single attribute.
3. Update one or more objects using the setter methods.
4. Display the updated values to verify the changes.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v; v.setMake("Ford"); v.setModel("Mustang"); v.setYear(2021); v.setMileage(60000.0f); v.displayVehicleInfo(); | Vehicle ID: empty, Make: Ford, Model: Mustang, Year: 2021, Mileage: 60000, Is Electric: 0, Transmission: empty, Engine Capacity: 0 |
| TC02 | Vehicle v; v.setMake("Hyundai"); v.setModel("Verna"); v.setYear(2023); v.setMileage(25000.0f); v.setEngineCapacity(1.6); v.displayVehicleInfo(); | Vehicle ID: empty, Make: Hyundai, Model: Verna, Year: 2023, Mileage: 25000, Is Electric: 0, Transmission: empty, Engine Capacity: 1.6 |
| TC03 | Vehicle v; v.setVehicleID("JKL012"); v.setMake("Kia"); v.setModel("Seltos"); v.setYear(2022); v.setMileage(33000.0f); v.displayVehicleInfo(); | Vehicle ID: JKL012, Make: Kia, Model: Seltos, Year: 2022, Mileage: 33000, Is Electric: 0, Transmission: empty, Engine Capacity: 0 |
| TC04 | Vehicle v; v.setIsElectric(true); v.setTransmissionType('A'); v.setMileage(1000.0f); v.displayVehicleInfo(); | Vehicle ID: empty, Make: empty, Model: empty, Year: 0, Mileage: 1000, Is Electric: 1, Transmission: A, Engine Capacity: 0 |
| TC05 | Vehicle v; v.setMake("Mahindra"); v.setModel("Thar"); v.setYear(2024); v.setMileage(7800.0f); v.setEngineCapacity(2.2); v.setIsElectric(false); v.displayVehicleInfo(); | Vehicle ID: empty, Make: Mahindra, Model: Thar, Year: 2024, Mileage: 7800, Is Electric: 0, Transmission: empty, Engine Capacity: 2.2 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the setter methods required for this question and demonstrates their use.
	- Required setter signatures to implement:
		- `void setVehicleID(const std::string& id);`
		- `void setMake(const std::string& make);`
		- `void setModel(const std::string& model);`
		- `void setYear(int year);` (validate reasonable year range)
		- `void setMileage(float mileage);` (validate non-negative)
		- `void setIsElectric(bool isElectric);`
		- `void setTransmissionType(char transmission);`
		- `void setEngineCapacity(double capacity);` (validate non-negative)
	- A small `main()` or test harness that uses these setters to reproduce the five provided test cases (TC01..TC05) and prints the resulting vehicle state.
	- Validation evidence (program output or brief test log) showing the produced output matches the Expected Output for each listed test case, plus at least one edge-case test demonstrating input validation.
	- Do not add or require other Vehicle methods, constructors, or APIs beyond what is needed to implement and demonstrate the setters for this question.

