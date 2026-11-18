# 31 - Sports Car Inheritance

## Introduction
Derived classes can add specialized performance attributes. A sports car typically has higher horsepower and different handling characteristics.

## Scenario
Implement a `SportsCar` derived from `Car` that includes performance metrics like horsepower and top speed, and add a method to compare performance between sports cars.

## Canonical Vehicle Attributes
The `SportsCar` derived class adds the following private members (use these exact names and types):
- `int horsepower` — engine output in horsepower
- `float topSpeed` — top speed in km/h

## Tasks to Implement
1. Create a SportsCar class derived from Car.
2. Add horsepower and topSpeed members.
3. Provide getter/setter methods for both properties.
4. Implement displaySportsCarInfo(SportsCar& sportsCar).

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | SportsCar sc("ABC123","Porsche","911",2023,10000.0f,false,'M',3.0); sc.setHorsepower(500); sc.setTopSpeed(300.5f); displaySportsCarInfo(sc); | Vehicle ID: ABC123, Make: Porsche, Model: 911, Horsepower: 500, Top Speed: 300.5 |
| TC02 | SportsCar sc("S1","Ferrari","F8",2024,3000.0f,false,'M',3.0); sc.setHorsepower(710); sc.setTopSpeed(340.0f); displaySportsCarInfo(sc); | Vehicle ID: S1, Make: Ferrari, Model: F8, Horsepower: 710, Top Speed: 340 |
| TC03 | SportsCar sc("S2","Lamborghini","Huracan",2023,8000.0f,false,'M',5.2); sc.setHorsepower(640); sc.setTopSpeed(325.0f); displaySportsCarInfo(sc); | Vehicle ID: S2, Make: Lamborghini, Model: Huracan, Horsepower: 640, Top Speed: 325 |
| TC04 | SportsCar sc("S3","McLaren","720S",2024,2500.0f,false,'M',4.0); sc.setHorsepower(710); sc.setTopSpeed(332.0f); displaySportsCarInfo(sc); | Vehicle ID: S3, Make: McLaren, Model: 720S, Horsepower: 710, Top Speed: 332 |
| TC05 | SportsCar sc("S4","Audi","R8",2022,20000.0f,false,'M',5.2); sc.setHorsepower(562); sc.setTopSpeed(204.0f); displaySportsCarInfo(sc); | Vehicle ID: S4, Make: Audi, Model: R8, Horsepower: 562, Top Speed: 204 |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add `SportsCar` derived class with `horsepower` and `topSpeed`, implement required methods, and display results).
- A short `main()` or test harness that constructs `SportsCar` objects, sets required fields, calls `displaySportsCarInfo()`, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

