# 01 - Vehicle Class Design and Properties

## Introduction
A vehicle record stores essential information such as the registration ID, make, model, year, mileage, and operating characteristics. This question focuses on designing a clear C++ class that keeps the data organized and exposes safe update methods.

## Scenario
A fleet management application must maintain vehicle records for cars used in transport and service operations. Each record should hold the vehicle ID, make, model, year, mileage, electric status, transmission type, and engine capacity. Implement the class so records can be created, updated, and displayed reliably.

## Tasks to Implement
1. Define a class named `Vehicle` that contains the following private data members (use these exact names and types):
	- `std::string vehicleID` — unique registration identifier
	- `std::string make`
	- `std::string model`
	- `int year`
	- `float mileage`
	- `bool isElectric`
	- `char transmissionType` (use `'A'` for automatic, `'M'` for manual)
	- `double engineCapacity`
2. Use the data types `std::string`, `int`, `float`, `bool`, `char`, and `double` for the fields.
3. (No setters required for this question.) The focus is on designing the class and its data members; implementation of setters/getters is out of scope.

## Test Cases

> Note: Test cases that exercise setters are out of scope for this question. If you implement constructors or display methods, you may create optional tests, but the primary goal here is class design.

## Suggested Validation Rules
- Verify the output matches the expected value for each valid test case.
- Check invalid or edge-case values such as negative years, zero mileage, empty strings, and invalid IDs.
- Ensure the implementation follows proper C++ OOP principles and clean coding standards.
- Confirm the behavior is correct for both stack and heap objects when applicable.

## Expected Deliverables
- A C++ class declaration named `Vehicle` that defines the required private data members exactly as listed above.
- A brief explanation (1-3 lines) of any design choices, if applicable (e.g., why `char` is used for `transmissionType`).
- Optional: a header file containing the class declaration. Do NOT include setter implementations for this question.

This question focuses strictly on class design and data members; implementation of setters/getters and other behaviors belongs to follow-up questions.