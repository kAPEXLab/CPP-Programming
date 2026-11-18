# 33 - Operator Overloading in Vehicle

## Introduction
Operator overloading makes user-defined types behave like built-ins for certain operations. This improves readability for domain-specific operations.

## Scenario
Overload operators such as `==` to compare vehicles by ID and `+` to combine mileage or other metrics, ensuring semantics are intuitive and well-documented.

## Tasks to Implement
1. Overload !, ==, +, =, >, and [].
2. Check whether the vehicle is not electric.
3. Compare by vehicle ID.
4. Add mileage of two vehicles.
5. Assign one object to another.
6. Compare engine capacities.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); bool equal = (v1 == v2); float totalMileage = v1 + v2; | equal = true, totalMileage = 100000 |
| TC02 | Vehicle v1("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); Vehicle v2("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0); bool equal = (v1 == v2); | equal = false |
| TC03 | Vehicle v1("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); Vehicle v2("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); float totalMileage = v1 + v2; | totalMileage = 136000 |
| TC04 | Vehicle v1("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); Vehicle v2("TESLA8","Tesla","Model X",2023,2000.0f,true,'A',0.0); bool equal = (v1 == v2); | equal = false |
| TC05 | Vehicle v1("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); Vehicle v2("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); bool equal = (v1 == v2); | equal = true |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (operator overloads specified and demonstration).
- A short `main()` or test harness that constructs sample vehicles, applies the overloaded operators, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

