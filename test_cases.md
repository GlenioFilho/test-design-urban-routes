# Equivalence Classes - Name

## 1. Nome

| **Nome da Classe**                 | **Limites**          | **Dados de Teste Dentro da Classe**                                   | **Dados de Teste nos Limites**               | **Classificação e Otimização**     |
|------------------------------------|----------------------|----------------------------------------------------------------------|---------------------------------------------|------------------------------------|
| Caracteres Especiais               | @, #, $, %           | "Maria@", "João#"                                                     | Contém caracteres especiais.               | Cenários negativos abrangidos.    |
| Símbolos                           | !, *, &, ^           | "Maria!", "João*"                                                     | Contém símbolos.                           | Cenários negativos abrangidos.    |
| Letras Latinas                     | A-Z, a-z             | "Maria", "João"                                                       | Contém letras latinas válidas.             | Entradas válidas agrupadas.       |
| Letras Não Latinas                 | кириллица, 汉字       | "Иван", "李华"                                                        | Contém letras não latinas.                 | Entradas inválidas agrupadas.     |
| Números                            | 0-9                  | "Maria123", "João456"                                                 | Contém números.                            | Entradas inválidas agrupadas.     |
| Campo com 1 Caractere             | 1                    | "A"                                                                   | Exatamente 1 caractere.                    | Cobertura de casos válidos e inválidos. |
| Campo com Texto entre 2 e 14 Caracteres | 2-14            | "João", "Ana-Maria"                                                   | Entre 2 e 14 caracteres.                   | Cobertura de limites de caracteres. |
| Campo com 15 ou Mais Caracteres    | 15 ou mais           | "Pedro Henrique Oliveira Silva"                                       | 15 ou mais caracteres.                     | Cobertura de limites máximos.     |
| Campo Vazio                        |                      | ""                                                                    | campo vazio.                               | Cobertura de campos vazios.      |

## 2. Sobrenome

| **Nome da Classe**                 | **Limites**          | **Dados de Teste Dentro da Classe**                                   | **Dados de Teste nos Limites**               | **Classificação e Otimização**     |
|------------------------------------|----------------------|----------------------------------------------------------------------|---------------------------------------------|------------------------------------|
| Caracteres Especiais               | @, #, $, %           | "Silva@", "De-Souza#"                                                 | Contém caracteres especiais.               | Cenários negativos abrangidos.    |
| Símbolos                           | !, *, &, ^           | "Silva!", "De-Souza*"                                                 | Contém símbolos.                           | Cenários negativos abrangidos.    |
| Letras Latinas                     | A-Z, a-z             | "Silva", "De Souza"                                                   | Contém letras latinas válidas.             | Entradas válidas agrupadas.       |
| Letras Não Latinas                 | кириллица, 汉字       | "Иванов", "张伟"                                                       | Contém letras não latinas.                 | Entradas inválidas agrupadas.     |
| Números                            | 0-9                  | "Silva123", "De-Souza456"                                             | Contém números.                            | Entradas inválidas agrupadas.     |
| Campo com 1 Caractere             | 1                    | "S"                                                                   | Exatamente 1 caractere.                    | Cobertura de casos válidos e inválidos. |
| Campo com Texto entre 2 e 14 Caracteres | 2-14            | "Silva", "De-Souza"                                                   | Entre 2 e 14 caracteres.                   | Cobertura de limites de caracteres. |
| Campo com 15 ou Mais Caracteres    | 15 ou mais           | "Fernandes Junior Monteiro"                                           | 15 ou mais caracteres.                     | Cobertura de limites máximos.     |
| Campo Vazio                        |                      | ""                                                                    | campo vazio.                               | Cobertura de campos vazios.      |

## 3. Data de Nascimento

| **Nome da Classe**                 | **Limites**          | **Dados de Teste Dentro da Classe**                                   | **Dados de Teste nos Limites**                    | **Classificação e Otimização**     |
|------------------------------------|----------------------|----------------------------------------------------------------------|--------------------------------------------------|------------------------------------|
| Dias Válidos                       | 01-31                | "01.01.2000", "29.02.2004", "30.04.1995"                              | Dias: 1, 28-31, meses válidos.                  | Entradas válidas cobertas.        |
| Meses Válidos                      | 01-12                | "01.01.2000", "12.12.1999"                                            | Meses: 1, 12, limites aceitos.                  | Entradas válidas cobertas.        |
| Anos Válidos                       | 1880-2006            | "1880", "2006"                                                        | Anos: 1880 e 2006 estão dentro dos limites.     | Anos válidos cobertos.            |
| Dias Inválidos                     | 00, 32               | "00.01.2000", "32.01.2000"                                            | Dias fora do limite (00, 32).                   | Cenários negativos abrangidos.    |
| Meses Inválidos                    | 00, 13               | "00.01.2000", "13.01.2000"                                            | Meses fora do limite (00, 13).                  | Cenários negativos abrangidos.    |
| Anos Inválidos                     | 1879, 2007           | "1879", "2007"                                                        | Anos fora do limite (1879, 2007).               | Cenários negativos abrangidos.    |
| Dia                                | 01-31                | "01.01.2000", "29.02.2004", "30.04.1995"                              | Dias válidos e limites.                         | Cobertura de datas válidas e inválidas. |
| Mês                                 | 01-12                | "01.01.2000", "12.12.1999"                                            | Meses válidos e limites.                        | Cobertura de meses válidos.      |
| Ano                                 | 1880-2006            | "1880", "2006"                                                        | Anos válidos e limites.                         | Cobertura de anos válidos.       |
| Letras Latinas                     | A-Z, a-z             | "Agosto"                                                              | Contém letras latinas.                          | Cobertura de letras inválidas.   |
| Letras Não Latinas                 | кириллица, 汉字       | "一九九一年五月一日"                                                   | Contém letras não latinas.                      | Cobertura de letras não latinas. |
| Símbolos                           | @, #, $, %           | "15@08#1990"                                                          | Contém símbolos.                                | Cobertura de símbolos inválidos. |
| Caracteres Especiais               | !, *, &, ^           | "15*08&1990"                                                          | Contém caracteres especiais.                    | Cobertura de caracteres especiais.|
| Campo Vazio                        |                      | ""                                                                    | campo vazio.                                    | Cobertura de campo vazio.        |
| Números                            | 0-9                  | "15081990"                                                            | Contém números.                                 | Cobertura de entradas numéricas. |
