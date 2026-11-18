# 40 - Driver Vehicle Association

## Introduction
Associations link different domain entities together, such as drivers and vehicles, to model relationships in a system.

## Scenario
Model a simple association between `Driver` and `Vehicle`, where a driver can be assigned to a vehicle. Provide methods to assign and unassign drivers and display associations.

## Canonical Vehicle Attributes
Refer to the canonical Vehicle attributes defined in Question 01. The `Driver` class required by this scenario should include the following members (use these exact names and types):
- `std::string driverName`
- `std::string driverLicenseNumber`
- `int yearsOfExperience`

Also, the `Vehicle` class should provide a way to record an assigned driver (e.g., `Driver* assignedDriver` or `std::optional<Driver>`). List only the additional members above; reuse other Vehicle members from Question 01.

## Tasks to Implement
1. Create a Driver class with driverName, driverLicenseNumber, and yearsOfExperience.
2. Implement assignVehicle(Vehicle vehicle) and getAssignedVehicle().
3. Implement assignDriver(Driver driver) and getAssignedDriver() inside Vehicle.
4. Demonstrate the association between both classes.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Driver driver("John Doe","DL12345",5); Vehicle v("ABC123","Toyota","Camry",2022,50000.0f,false,'A',2.5); driver.assignVehicle(v); v.assignDriver(driver); | Assigned driver and vehicle are displayed successfully. |
| TC02 | Driver driver("Alice Smith","DL67890",8); Vehicle v("XYZ999","Honda","Civic",2021,45000.0f,false,'M',1.8); driver.assignVehicle(v); v.assignDriver(driver); | Assigned driver and vehicle are displayed successfully. |
| TC03 | Driver driver("Robert Lee","DL22222",6); Vehicle v("BMW77","BMW","X5",2020,68000.0f,false,'A',3.0); driver.assignVehicle(v); v.assignDriver(driver); | Assigned driver and vehicle are displayed successfully. |
| TC04 | Driver driver("Priya Shah","DL33333",4); Vehicle v("TESLA7","Tesla","Model Y",2024,1500.0f,true,'A',0.0); driver.assignVehicle(v); v.assignDriver(driver); | Assigned driver and vehicle are displayed successfully. |
| TC05 | Driver driver("Daniel Roy","DL44444",10); Vehicle v("AUDI08","Audi","A4",2019,74000.0f,false,'M',2.0); driver.assignVehicle(v); v.assignDriver(driver); | Assigned driver and vehicle are displayed successfully. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (implement `Driver` class, `Vehicle` driver-assignment methods, and demonstrate associations).
- Implement the `Driver` class with the following public API:
	- `Driver();`
	- `Driver(const std::string& driverName, const std::string& driverLicenseNumber, int yearsOfExperience);`
	- `std::string getDriverName() const;` / `void setDriverName(const std::string&);`
	- `std::string getDriverLicenseNumber() const;` / `void setDriverLicenseNumber(const std::string&);`
	- `int getYearsOfExperience() const;` / `void setYearsOfExperience(int);`
- Add the following `Vehicle` methods required by this question (only these):
	- `void assignDriver(const Driver& driver);`
	- `void unassignDriver();`
	- `const Driver* getAssignedDriver() const;`
- A short `main()` or test harness that constructs `Driver` and `Vehicle` objects, calls `assignDriver()` / `assignVehicle()`, and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing outputs match the Expected Output for each test case.

