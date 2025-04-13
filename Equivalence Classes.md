# Equivalence Classes for Data Validation

## Overview
Equivalence Partitioning is a technique used in software testing to identify equivalent groups of inputs, which allows us to test representative values from each group. This method helps in reducing the number of test cases while ensuring all possible inputs are covered effectively. Below is a breakdown of the equivalence classes for the "Name", "Surname", and "Date of Birth" fields.

---

## Nome (Name)

| **Verification Group**        | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data at the Limits**        | **Classification and Optimization** |
|-------------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Special Characters            | Special Characters          | @, #, $, %               | "Maria@", "João#"                      |                                    | Contains special characters. Covered negative scenarios. |
| Symbols                       | Symbols                     | !, *, &, ^               | "Maria!", "João*"                      |                                    | Contains symbols. Covered negative scenarios. |
| Latin Letters                 | Latin Letters               | A-Z, a-z                 | "Maria", "João"                        |                                    | Contains valid Latin letters. Valid entries grouped. |
| Non-Latin Letters             | Non-Latin Letters           | кириллица, 汉字           | "Иван", "李华"                         |                                    | Contains non-Latin letters. Invalid entries grouped. |
| Numbers                       | Numbers                     | 0-9                      | "Maria123", "João456"                  |                                    | Contains numbers. Invalid entries grouped. |
| 1 Character Field             | 1 Character                 | 1                        | "A"                                    |                                    | Exactly 1 character. Coverage of valid and invalid cases. |
| Text Field 2-14 Characters    | 2-14 Characters             | 2-14                     | "João", "Ana-Maria"                    |                                    | Between 2 and 14 characters. Coverage of character limits. |
| 15 or More Characters         | 15 or More                  | 15 or More               | "Pedro Henrique Oliveira Silva"        |                                    | Coverage of maximum limits. |
| Empty Field                   | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |

---

## Sobrenome (Surname)

| **Verification Group**        | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data at the Limits**        | **Classification and Optimization** |
|-------------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Special Characters            | Special Characters          | @, #, $, %               | "Silva@", "De-Souza#"                  |                                    | Contains special characters. Covered negative scenarios. |
| Symbols                       | Symbols                     | !, *, &, ^               | "Silva!", "De-Souza*"                  |                                    | Contains symbols. Covered negative scenarios. |
| Latin Letters                 | Latin Letters               | A-Z, a-z                 | "Silva", "De Souza"                    |                                    | Contains valid Latin letters. Valid entries grouped. |
| Non-Latin Letters             | Non-Latin Letters           | кириллица, 汉字           | "Иванов", "张伟"                       |                                    | Contains non-Latin letters. Invalid entries grouped. |
| Numbers                       | Numbers                     | 0-9                      | "Silva123", "De-Souza456"              |                                    | Contains numbers. Invalid entries grouped. |
| 1 Character Field             | 1 Character                 | 1                        | "S"                                    |                                    | Exactly 1 character. Coverage of valid and invalid cases. |
| Text Field 2-14 Characters    | 2-14 Characters             | 2-14                     | "Silva", "De-Souza"                    |                                    | Between 2 and 14 characters. Coverage of character limits. |
| 15 or More Characters         | 15 or More                  | 15 or More               | "Fernandes Junior Monteiro"            |                                    | Coverage of maximum limits. |
| Empty Field                   | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |

---

## Data de Nascimento (Date of Birth)

| **Verification Group**        | **Class Name**              | **Limits**               | **Test Data within the Class**         | **Test Data at the Limits**        | **Classification and Optimization** |
|-------------------------------|-----------------------------|--------------------------|----------------------------------------|------------------------------------|------------------------------------|
| Valid Days                    | Valid Days                  | 01-31                    | "01.01.2000", "29.02.2004", "30.04.1995" |                                    | Days: 1, 28-31, valid days. |
| Valid Months                  | Valid Months                | 01-12                    | "01.01.2000", "12.12.1999"             |                                    | Months: 1-12, valid months. |
| Valid Years                   | Valid Years                 | 1880-2006                | "1880", "2006"                         |                                    | Years: 1880-2006, valid years. |
| Invalid Days                  | Invalid Days                | 00, 32                   | "00.01.2000", "32.01.2000"             |                                    | Invalid days: 00, 32. |
| Invalid Months                | Invalid Months              | 00, 13                   | "00.01.2000", "13.01.2000"             |                                    | Invalid months: 00, 13. |
| Invalid Years                 | Invalid Years               | 1879, 2007               | "1879", "2007"                         |                                    | Invalid years: 1879, 2007. |
| Day                           | Valid Day                   | 0, 1, 2, 27-32           | "01.01.2000", "29.02.2004", "30.04.1995" |                                    | Valid days and limits covered. |
| Month                         | Valid Month                 | 0, 1, 2, 11, 12, 13       | "01.01.2000", "12.12.1999"             |                                    | Valid months and limits covered. |
| Year                          | Valid Year                  | 1879, 1880, 1881, 2005, 2006, 2007 | "1880", "2006"                    |                                    | Valid years and limits covered. |
| Latin Letters                 | Latin Letters               | A-Z, a-z                 | "Agosto"                               |                                    | Contains Latin letters. Coverage of invalid letters. |
| Non-Latin Letters             | Non-Latin Letters           | Не латиница, 汉字          | "一九九一年五月一日"                    |                                    | Contains non-Latin letters. Coverage of invalid letters. |
| Symbols                       | Symbols                     | @, #, $, %               | "15@08#1990"                           |                                    | Contains symbols. Coverage of invalid symbols. |
| Special Characters            | Special Characters          | !, *, &, ^               | "15*08&1990"                           |                                    | Contains special characters. Coverage of special characters. |
| Empty Field                   | Empty Field                 | ""                       | ""                                     |                                    | Coverage of empty fields. |
| Numbers                       | Numbers                     | 0-9                      | "15081990"                             |                                    | Contains numbers. Coverage of numerical entries. |

---

## Conclusion

This documentation covers the **Equivalence Classes** for data validation of Name, Surname, and Date of Birth fields. These classes help us optimize testing by focusing on a representative set of inputs rather than testing every possible combination. Each class is designed to cover both valid and invalid input scenarios, as well as boundary conditions, ensuring that the application behaves correctly across all expected inputs.

This structure helps reduce the number of test cases while still ensuring a comprehensive test of the input validation logic. By categorizing inputs into equivalence classes, we can ensure that the system is tested efficiently and effectively.

