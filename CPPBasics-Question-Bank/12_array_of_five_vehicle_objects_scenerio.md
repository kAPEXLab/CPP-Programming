# 12 - Array of Five Vehicle Objects

## Introduction
Arrays provide contiguous storage for multiple objects. This question focuses on creating arrays of objects and iterating over them.

## Scenario
Create an array of five `Vehicle` objects, initialize each entry, and implement logic to process and display all records (for example, computing average mileage).

## Tasks to Implement
1. Create an array of five Vehicle objects.
2. Initialize each object with a unique vehicle record.
3. Loop through the array and print each object.
4. Verify that all five records are displayed.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle vehicles[5] = { Vehicle("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5), Vehicle("DEF456","Ford","Mustang",2021,60000.0f,false,'M',3.0), Vehicle("GHI789","Honda","Civic",2020,70000.0f,false,'A',2.0), Vehicle("JKL012","Tesla","Model S",2019,80000.0f,true,'A',0.0), Vehicle("MNO345","VW","Golf",2018,90000.0f,false,'M',2.0) }; | Five vehicle records printed successfully. |
| TC02 | Vehicle vehicles[5] = { Vehicle("A1","Renault","Kwid",2021,36000.0f,false,'M',1.0), Vehicle("A2","Maruti","Swift",2022,28000.0f,false,'A',1.2), Vehicle("A3","MG","Hector",2023,20000.0f,false,'A',2.0), Vehicle("A4","Tata","Nexon",2020,47000.0f,false,'M',1.5), Vehicle("A5","Kia","Sonet",2024,12000.0f,false,'A',1.5) }; | Five vehicle records printed successfully. |
| TC03 | Vehicle vehicles[5] = { Vehicle("V1","Ford","Figo",2019,54000.0f,false,'M',1.2), Vehicle("V2","Chevrolet","Beat",2018,61000.0f,false,'M',1.2), Vehicle("V3","Skoda","Rapid",2021,44000.0f,false,'A',1.4), Vehicle("V4","Hyundai","Creta",2023,17000.0f,false,'A',1.5), Vehicle("V5","Mahindra","Scorpio",2022,25000.0f,false,'M',2.2) }; | Five vehicle records printed successfully. |
| TC04 | Vehicle vehicles[5] = { Vehicle("C1","Toyota","Innova",2020,52000.0f,false,'A',2.8), Vehicle("C2","Honda","City",2021,42000.0f,false,'M',1.5), Vehicle("C3","Nissan","Micra",2018,72000.0f,false,'M',1.2), Vehicle("C4","Tesla","Model 3",2024,15000.0f,true,'A',0.0), Vehicle("C5","Mercedes","C-Class",2022,33000.0f,false,'A',2.0) }; | Five vehicle records printed successfully. |
| TC05 | Vehicle vehicles[5] = { Vehicle("S1","Volvo","XC60",2021,35000.0f,false,'A',2.0), Vehicle("S2","Peugeot","208",2023,18000.0f,false,'M',1.3), Vehicle("S3","Mini","Cooper",2022,30000.0f,false,'A',2.0), Vehicle("S4","Porsche","Macan",2024,9000.0f,false,'A',2.9), Vehicle("S5","Audi","Q5",2020,65000.0f,false,'M',2.0) }; | Five vehicle records printed successfully. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (create and display an array of five `Vehicle` objects).
- A short `main()` or test harness that constructs an array of five `Vehicle` objects, initializes them, and prints their state to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

