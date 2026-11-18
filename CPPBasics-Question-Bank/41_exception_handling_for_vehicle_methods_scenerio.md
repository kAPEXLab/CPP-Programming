# 41 - Exception Handling for Vehicle Methods

## Introduction
Robust code handles invalid input and runtime errors gracefully. Exception handling provides a structured way to signal and manage errors.

## Scenario
Update vehicle methods to throw and catch exceptions for invalid operations (e.g., negative mileage, invalid year) and demonstrate safe usage with try/catch blocks.

## Tasks to Implement
1. Add try/catch blocks in setter methods and other functions.
2. Handle bad input such as negative mileage and invalid year values.
3. Use std::exception or custom exceptions to report the issue.
4. Ensure the program continues running after the exception is handled.

## Test Cases

| Test Case ID | Input | Expected Output |
| --- | --- | --- |
| TC01 | Vehicle v; try { v.setYear(-2020); } catch (const std::exception& e) { std::cout << e.what(); } | Invalid vehicle year. |
| TC02 | Vehicle v; try { v.setMileage(-500.0f); } catch (const std::exception& e) { std::cout << e.what(); } | Invalid vehicle mileage. |
| TC03 | Vehicle v; try { v.setEngineCapacity(-1.5); } catch (const std::exception& e) { std::cout << e.what(); } | Invalid engine capacity. |
| TC04 | Vehicle v; try { v.setVehicleID(""); } catch (const std::exception& e) { std::cout << e.what(); } | Invalid vehicle ID. |
| TC05 | Vehicle v; try { v.setYear(0); } catch (const std::exception& e) { std::cout << e.what(); } | Invalid vehicle year. |

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ solution that implements only the items required by this question's "Tasks to Implement" (add exception handling to setters and demonstrate try/catch usage).
- Implement setter methods to throw `std::invalid_argument` (or an appropriate `std::exception` subclass) with clear messages for invalid inputs, for example:
	- `void setYear(int year); // throws std::invalid_argument("Invalid vehicle year.")`
	- `void setMileage(float mileage); // throws std::invalid_argument("Invalid vehicle mileage.")`
	- `void setEngineCapacity(double capacity); // throws std::invalid_argument("Invalid engine capacity.")`
	- `void setVehicleID(const std::string& id); // throws std::invalid_argument("Invalid vehicle ID.")`
- A short `main()` or test harness that calls the setters inside `try`/`catch` blocks and reproduces the provided test cases (TC01..TC05).
- Validation evidence (program output or brief test log) showing the exception messages match the Expected Output for each test case.

