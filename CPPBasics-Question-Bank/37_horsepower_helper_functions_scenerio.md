# 37 - Horsepower Helper Functions

## Introduction
Helper functions simplify repeated logic, such as calculating derived properties like horsepower-based performance ratings.

## Scenario
Implement helper functions that compute derived metrics (e.g., performance score based on horsepower and weight) and demonstrate their use with vehicle instances.
## Canonical Vehicle Attributes

This scenario depends on vehicles exposing horsepower — either by including an `Engine engine` member (see Question 36) with an `int horsepower` field or by providing `int getHorsepower()` on `Vehicle`.

If using composition, ensure `Engine` has at least `int horsepower` accessible to the helper functions.

## Tasks to Implement
1. Implement int getHorsepower(Vehicle vehicle).
2. Implement void increaseHorsepower(Vehicle& vehicle, int amount).
3. Implement void decreaseHorsepower(Vehicle& vehicle, int amount).
4. Implement int compareHorsepower(Vehicle vehicle1, Vehicle vehicle2).
5. Use the helper functions on sample vehicles.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); increaseHorsepower(v1,30); compareHorsepower(v1,v2); | Horsepower increased and then compared successfully. |
| TC02 | Vehicle v1("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); decreaseHorsepower(v1,20); std::cout << getHorsepower(v1); | Horsepower decreased successfully. |
| TC03 | Vehicle v1("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); increaseHorsepower(v1,50); std::cout << getHorsepower(v1); | Horsepower increased successfully. |
| TC04 | Vehicle v1("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle v2("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); compareHorsepower(v1,v2); | Horsepower values are equal. |
| TC05 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); compareHorsepower(v1,v2); | Horsepower comparison completed. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement the helper functions operating on vehicle horsepower and demonstrate them).
- Implement the following functions with these signatures:
	- `int getHorsepower(const Vehicle& vehicle);`
	- `void increaseHorsepower(Vehicle& vehicle, int amount);`
	- `void decreaseHorsepower(Vehicle& vehicle, int amount);`
	- `int compareHorsepower(const Vehicle& vehicle1, const Vehicle& vehicle2);`
- A short `main()` or test harness that constructs sample vehicles, calls these helper functions, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

