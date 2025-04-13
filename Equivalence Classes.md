# Equivalence Classes Descriptions

The following test cases were designed to validate the correct functioning of the data input system. The goal is to ensure the system properly validates fields such as name, surname, and date of birth according to the defined validation rules. Each test case follows a set of preconditions, steps to be executed, and the expected results to ensure data integrity.

# Equivalence Classes

| **Test Case ID** | **Test Case Name**         | **Pre-condition**                             | **Step Number** | **Step Description**                                                   | **Expected Result**                                                    |
|------------------|----------------------------|-----------------------------------------------|-----------------|------------------------------------------------------------------------|------------------------------------------------------------------------|
| t-1              | Empty "Name" Field         | The "Name" field must be empty                | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the field is required.       |
|                  |                            |                                               | 2               | Leave the "Name" field empty.                                           |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-2              | Text with 1 Character      | The "Name" field must have 1 character        | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the name must have at least 2 characters. |
|                  |                            |                                               | 2               | Enter "A" in the "Name" field.                                         |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-3              | Text with 2 Characters     | The "Name" field must have 2 characters       | 1               | Navigate to the "Add Driver's License" form.                           | Accepts the input without errors.                                      |
|                  |                            |                                               | 2               | Enter "Jo" in the "Name" field.                                        |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-4              | Text with 3 Characters     | The "Name" field must have 3 characters       | 1               | Navigate to the "Add Driver's License" form.                           | Accepts the input without errors.                                      |
|                  |                            |                                               | 2               | Enter "Ana" in the "Name" field.                                       |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-5              | Text with 13 Characters    | The "Name" field must have 13 characters      | 1               | Navigate to the "Add Driver's License" form.                           | Accepts the input without errors.                                      |
|                  |                            |                                               | 2               | Enter "Carlos Monte" in the "Name" field.                              |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-6              | Text with 14 Characters    | The "Name" field must have 14 characters      | 1               | Navigate to the "Add Driver's License" form.                           | Accepts the input without errors.                                      |
|                  |                            |                                               | 2               | Enter "Maria-Silva" in the "Name" field.                               |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-7              | Text with 15 Characters    | The "Name" field must have 15 characters      | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the name exceeds 14 characters. |
|                  |                            |                                               | 2               | Enter "Thiago Henrique" in the "Name" field.                           |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |

## Test Cases - Surname

| **Test Case ID** | **Test Case Name**         | **Pre-condition**                             | **Step Number** | **Step Description**                                                   | **Expected Result**                                                    |
|------------------|----------------------------|-----------------------------------------------|-----------------|------------------------------------------------------------------------|------------------------------------------------------------------------|
| t-1              | Empty "Surname" Field      | The "Surname" field must be empty             | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the field is required.       |
|                  |                            |                                               | 2               | Leave the "Surname" field empty.                                        |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-2              | Text with 1 Character      | The "Surname" field must have 1 character     | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the surname must have at least 2 characters. |
|                  |                            |                                               | 2               | Enter "S" in the "Surname" field.                                      |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |

## Test Cases - Date of Birth

| **Test Case ID** | **Test Case Name**         | **Pre-condition**                             | **Step Number** | **Step Description**                                                   | **Expected Result**                                                    |
|------------------|----------------------------|-----------------------------------------------|-----------------|------------------------------------------------------------------------|------------------------------------------------------------------------|
| t-1              | Valid Date of Birth        | The date of birth must be valid               | 1               | Navigate to the "Add Driver's License" form.                           | Accepts the input without errors.                                      |
|                  |                            |                                               | 2               | Enter "01.01.2000" in the "Date of Birth" field.                       |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |
| t-2              | Invalid Date of Birth      | The date of birth must be invalid             | 1               | Navigate to the "Add Driver's License" form.                           | Displays an error message indicating that the date is invalid.         |
|                  |                            |                                               | 2               | Enter "32.13.2000" in the "Date of Birth" field.                       |                                                                        |
|                  |                            |                                               | 3               | Remove focus from the field by clicking outside of it.                 |                                                                        |

---

## Conclusion

The test cases provided above were created to ensure that all input fields (name, surname, and date of birth) function as expected. Every valid or invalid input is tested, including boundary cases and values outside the expected range, to cover all possibilities and ensure the integrity of the data validation system.
