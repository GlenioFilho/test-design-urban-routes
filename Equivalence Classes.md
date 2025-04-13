# Equivalence Classes for Data Validation

## Overview
Equivalence Partitioning is a software testing technique used to reduce the number of test cases to a manageable level while ensuring coverage of all possible input scenarios. The goal is to divide inputs into classes that are treated the same by the system, allowing us to test representative values from each class rather than testing all possible inputs.

### Equivalence Classes for the "Name" Field

| **Verification Group**   | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data on the Limits**        | **Classification and Optimization** |
|--------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Special Characters       | Special Characters          | @, #, $, %               | "Maria@", "João#"                      |                                    | Contains special characters. Covered negative scenarios. |
| Symbols                  | Symbols                     | !, *, &, ^               | "Maria!", "João*"                      |                                    | Contains symbols. Covered negative scenarios. |
| Latin Letters            | Latin Letters               | A-Z, a-z                 | "Maria", "João"                        |                                    | Contains valid Latin letters. Valid entries grouped. |
| Non-Latin Letters        | Non-Latin Letters           | кириллица, 汉字           | "Иван", "李华"                         |                                    | Contains non-Latin letters. Invalid entries grouped. |
| Numbers                  | Numbers                     | 0-9                      | "Maria123", "João456"                  |                                    | Contains numbers. Invalid entries grouped. |
| 1 Character Field        | 1 Character                 | 1                        | "A"                                    |                                    | Exactly 1 character. Coverage of valid and invalid cases. |
| Text Field 2-14 Characters | 2-14 Characters            | 2-14                     | "João", "Ana-Maria"                    |                                    | Between 2 and 14 characters. Coverage of character limits. |
| 15 or More Characters    | 15 or More                  | 15 or More               | "Pedro Henrique Oliveira Silva"        |                                    | Coverage of maximum limits. |
| Empty Field              | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |

### Equivalence Classes for the "Surname" Field

| **Verification Group**   | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data on the Limits**        | **Classification and Optimization** |
|--------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Special Characters       | Special Characters          | @, #, $, %               | "Silva@", "De-Souza#"                  |                                    | Contains special characters. Covered negative scenarios. |
| Symbols                  | Symbols                     | !, *, &, ^               | "Silva!", "De-Souza*"                  |                                    | Contains symbols. Covered negative scenarios. |
| Latin Letters            | Latin Letters               | A-Z, a-z                 | "Silva", "De Souza"                    |                                    | Contains valid Latin letters. Valid entries grouped. |
| Non-Latin Letters        | Non-Latin Letters           | кириллица, 汉字           | "Иванов", "张伟"                       |                                    | Contains non-Latin letters. Invalid entries grouped. |
| Numbers                  | Numbers                     | 0-9                      | "Silva123", "De-Souza456"              |                                    | Contains numbers. Invalid entries grouped. |
| 1 Character Field        | 1 Character                 | 1                        | "S"                                    |                                    | Exactly 1 character. Coverage of valid and invalid cases. |
| Text Field 2-14 Characters | 2-14 Characters            | 2-14                     | "Silva", "De-Souza"                    |                                    | Between 2 and 14 characters. Coverage of character limits. |
| 15 or More Characters    | 15 or More                  | 15 or More               | "Fernandes Junior Monteiro"            |                                    | Coverage of maximum limits. |
| Empty Field              | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |

### Equivalence Classes for the "Date of Birth" Field

| **Verification Group**   | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data on the Limits**        | **Classification and Optimization** |
|--------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Days                     | Valid Days                  | 01-31                    | "01.01.2000", "29.02.2004"             | "30.04.1995"                      | Days: 1, 28-31, valid days. |
| Months                   | Valid Months                | 01-12                    | "01.01.2000", "12.12.1999"             |                                    | Months: 1-12, valid months. |
| Years                    | Valid Years                 | 1880-2006                | "1880", "2006"                         |                                    | Years: 1880-2006, valid years. |
| Days                     | Invalid Days                | 00, 32                   | "00.01.2000", "32.01.2000"             |                                    | Invalid days: 00, 32. |
| Months                   | Invalid Months              | 00, 13                   | "00.01.2000", "13.01.2000"             |                                    | Invalid months: 00, 13. |
| Years                    | Invalid Years               | 1879, 2007               | "1879", "2007"                         |                                    | Invalid years: 1879, 2007. |
| Text                     | Invalid Text                | A-Z, a-z                 | "Agosto"                               |                                    | Contains non-numeric characters. |
| Symbols                  | Invalid Symbols             | @, #, $, %               | "15@08#1990"                           |                                    | Contains symbols. |
| Numbers                  | Numbers                     | 0-9                      | "15081990"                             |                                    | Valid number format for date. |
| Empty                    | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |
