# 39 - Transmission Type Enumeration

## Introduction
Enumerations provide clear named constants for a limited set of values, improving readability and reducing invalid inputs.

## Scenario
Define an `enum` for transmission types (e.g., `Manual`, `Automatic`, `CVT`) and use it in `Vehicle` to restrict transmission values and simplify checks.

## Canonical Vehicle Attributes
Refer to the canonical Vehicle attributes defined in Question 01. For this scenario replace the `char transmissionType` member with an enumeration:
- `enum class TransmissionType { MANUAL, AUTOMATIC, SEMI_AUTOMATIC, CONTINUOUSLY_VARIABLE_TRANSMISSION, CVT }` 
- `TransmissionType transmissionType` — use the enum instead of a `char` for clearer semantics

## Tasks to Implement
1. Define `enum class TransmissionType { MANUAL, AUTOMATIC, SEMI_AUTOMATIC, CONTINUOUSLY_VARIABLE_TRANSMISSION, CVT };`
2. Add the `TransmissionType transmissionType` property to `Vehicle`.
3. Implement `displayVehicleInfo()` to print the transmission type as a readable name.
4. Create `TransmissionType getTransmissionType(const Vehicle&);` and `void setTransmissionType(Vehicle&, TransmissionType);`.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v("ABC123","Toyota","Camry",2022,50000.0f,false,TransmissionType::AUTOMATIC,2.5); displayVehicleInfo(v); | Transmission Type: AUTOMATIC |
| TC02 | Vehicle v("XYZ999","Honda","Civic",2021,45000.0f,false,TransmissionType::MANUAL,1.8); displayVehicleInfo(v); | Transmission Type: MANUAL |
| TC03 | Vehicle v("BMW77","BMW","X5",2020,68000.0f,false,TransmissionType::SEMI_AUTOMATIC,3.0); displayVehicleInfo(v); | Transmission Type: SEMI_AUTOMATIC |
| TC04 | Vehicle v("TESLA7","Tesla","Model Y",2024,1500.0f,true,TransmissionType::CONTINUOUSLY_VARIABLE_TRANSMISSION,0.0); displayVehicleInfo(v); | Transmission Type: CONTINUOUSLY_VARIABLE_TRANSMISSION |
| TC05 | Vehicle v("AUDI08","Audi","A4",2019,74000.0f,false,TransmissionType::AUTOMATIC,2.0); displayVehicleInfo(v); | Transmission Type: AUTOMATIC |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (define the `TransmissionType` enum, add property to `Vehicle`, provide getter/setter and display behavior).
- Provide the following API elements (only these are required by this question):
	- `enum class TransmissionType { MANUAL, AUTOMATIC, SEMI_AUTOMATIC, CONTINUOUSLY_VARIABLE_TRANSMISSION, CVT };`
	- `TransmissionType getTransmissionType(const Vehicle& vehicle);`
	- `void setTransmissionType(Vehicle& vehicle, TransmissionType type);`
	- `void displayVehicleInfo() const;` (must print the transmission type name)
- A short `main()` or test harness that constructs `Vehicle` objects using the enum for transmission and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

