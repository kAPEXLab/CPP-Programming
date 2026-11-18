# 14 - Three Additional Heap Vehicle Objects

## Introduction
Dynamically expanding storage lets programs handle more items than fixed-size arrays. This exercise practices allocating additional heap objects when needed.

## Scenario
Start with a base array of vehicles, then dynamically allocate three additional `Vehicle` objects on the heap and add them to a pointer-based list. Demonstrate correct allocation and cleanup.

## Tasks to Implement
1. Create three Vehicle instances with new.
2. Initialize them with the given values.
3. Display each one with displayVehicleInfo().
4. Delete all three objects after use.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle* p1 = new Vehicle("PQR678","Nissan","Altima",2023,40000.0f,false,'A',2.2); Vehicle* p2 = new Vehicle("STU901","BMW","3-Series",2022,55000.0f,false,'M',2.8); Vehicle* p3 = new Vehicle("VWX234","Audi","A4",2021,65000.0f,false,'A',2.0); p1->displayVehicleInfo(); p2->displayVehicleInfo(); p3->displayVehicleInfo(); delete p1; delete p2; delete p3; | Three vehicle objects are displayed and deleted successfully. |
| TC02 | Vehicle* p1 = new Vehicle("V1","Toyota","Fortuner",2022,32000.0f,false,'A',2.8); Vehicle* p2 = new Vehicle("V2","Honda","CR-V",2021,42000.0f,false,'A',1.5); Vehicle* p3 = new Vehicle("V3","Ford","Endeavour",2023,26000.0f,false,'M',3.0); p1->displayVehicleInfo(); delete p1; delete p2; delete p3; | Three vehicle objects are displayed and deleted successfully. |
| TC03 | Vehicle* p1 = new Vehicle("E1","Tesla","Model S",2024,11000.0f,true,'A',0.0); Vehicle* p2 = new Vehicle("E2","Tesla","Model X",2024,9000.0f,true,'A',0.0); Vehicle* p3 = new Vehicle("E3","Tesla","Model Y",2023,14000.0f,true,'A',0.0); p2->displayVehicleInfo(); delete p1; delete p2; delete p3; | Three vehicle objects are displayed and deleted successfully. |
| TC04 | Vehicle* p1 = new Vehicle("H1","Hyundai","Creta",2021,45000.0f,false,'M',1.5); Vehicle* p2 = new Vehicle("H2","Hyundai","Venue",2022,30000.0f,false,'A',1.2); Vehicle* p3 = new Vehicle("H3","Hyundai","Verna",2020,54000.0f,false,'M',1.6); p3->displayVehicleInfo(); delete p1; delete p2; delete p3; | Three vehicle objects are displayed and deleted successfully. |
| TC05 | Vehicle* p1 = new Vehicle("M1","Mahindra","Thar",2024,7500.0f,false,'M',2.0); Vehicle* p2 = new Vehicle("M2","Mahindra","XUV700",2023,18000.0f,false,'A',2.2); Vehicle* p3 = new Vehicle("M3","Mahindra","Bolero",2021,61000.0f,false,'M',1.9); p1->displayVehicleInfo(); delete p1; delete p2; delete p3; | Three vehicle objects are displayed and deleted successfully. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (allocate three additional `Vehicle` objects on the heap, display, and clean up).
- A short `main()` or test harness that allocates three `Vehicle` objects with `new`, demonstrates their use, prints their state, and deletes them to reproduce the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case and that `delete` was called for each allocated object.

