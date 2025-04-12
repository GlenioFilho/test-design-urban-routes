# Equivalence Classes - Name

| Verification Group        | Class Name         | Limits                | Test Data within the Class   | Test Data on the Limits         | Classification and Optimization                |
|---------------------------|--------------------|-----------------------|------------------------------|---------------------------------|------------------------------------------------|
| Special Characters         | Special Characters | @, #, $, %            | "Maria@", "João#"            | Contains special characters.    | Covered negative scenarios.                   |
| Symbols                   | Symbols            | !, *, &, ^            | "Maria!", "João*"            | Contains symbols.               | Covered negative scenarios.                   |
| Latin Letters              | Latin Letters      | A-Z, a-z              | "Maria", "João"              | Contains valid Latin letters.   | Valid entries grouped.                        |
| Non-Latin Letters          | Non-Latin Letters  | кириллица, 汉字        | "Иван", "李华"               | Contains non-Latin letters.     | Invalid entries grouped.                      |
| Numbers                    | Numbers            | 0-9                   | "Maria123", "João456"        | Contains numbers.               | Invalid entries grouped.                      |
| 1 Character Field          | 1 Character        | 1                     | "A"                          | Exactly 1 character.            | Coverage of valid and invalid cases.          |
| Text Field 2-14 Characters | 2-14               |                       | "João", "Ana-Maria"          | Between 2 and 14 characters.    | Coverage of character limits.                 |
| 15 or More Characters Field| 15 or More         |                       | "Pedro Henrique Oliveira Silva" | 15 or more characters.         | Coverage of maximum limits.                   |
| Empty Field                | Empty Field        | ""                    | ""                           | Empty field.                    | Coverage of empty fields.                     |

# Test Cases - Name

| Test Case ID | Test Case Name        | Pre-condition                               | Step Number | Step Description                                 | Expected Result                                                         |
|--------------|-----------------------|--------------------------------------------|-------------|-------------------------------------------------|------------------------------------------------------------------------|
| t-1          | Empty "NAME" Field     | The 'Name' field must be empty             | 1           | Navigate to the 'Add Driver's License' form.    | Displays an error message indicating that the field is required.      |
|              |                       |                                            | 2           | Leave the 'Name' field empty.                   |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-2          | Text with 1 Character  | The 'Name' field must have 1 character     | 1           | Navigate to the 'Add Driver's License' form.    | Displays an error message indicating that the name must have at least 2 characters. |
|              |                       |                                            | 2           | Enter 'A' in the 'Name' field.                 |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-3          | Text with 2 Characters | The 'Name' field must have 2 characters    | 1           | Navigate to the 'Add Driver's License' form.    | Accepts the input without errors.                                      |
|              |                       |                                            | 2           | Enter 'Jo' in the 'Name' field.                |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-4          | Text with 3 Characters | The 'Name' field must have 3 characters    | 1           | Navigate to the 'Add Driver's License' form.    | Accepts the input without errors.                                      |
|              |                       |                                            | 2           | Enter 'Ana' in the 'Name' field.               |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-5          | Text with 13 Characters| The 'Name' field must have 13 characters   | 1           | Navigate to the 'Add Driver's License' form.    | Accepts the input without errors.                                      |
|              |                       |                                            | 2           | Enter 'Carlos Monte' in the 'Name' field.       |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-6          | Text with 14 Characters| The 'Name' field must have 14 characters   | 1           | Navigate to the 'Add Driver's License' form.    | Accepts the input without errors.                                      |
|              |                       |                                            | 2           | Enter 'Maria-Silva' in the 'Name' field.        |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |
| t-7          | Text with 15 Characters| The 'Name' field must have 15 characters   | 1           | Navigate to the 'Add Driver's License' form.    | Displays an error message indicating that the name exceeds 14 characters. |
|              |                       |                                            | 2           | Enter 'Thiago Henrique' in the 'Name' field.    |                                                                        |
|              |                       |                                            | 3           | Remove focus from the field by clicking outside of it. |                                                                        |

