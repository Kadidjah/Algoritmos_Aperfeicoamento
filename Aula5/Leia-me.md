# Aula 05 - Tomada de Decisão II
## Tema: Operadores lógicos (E, OU, NÃO) e condições encadeadas
### Prática: Classificação de atletas por idade

---

## Objetivo
Aprender a utilizar operadores lógicos e condições encadeadas para resolver problemas mais complexos de decisão.

---

## Exposição Teórica (15 min)
- **Operadores Lógicos:**
  - **E (AND):** todas as condições precisam ser verdadeiras.
  - **OU (OR):** basta uma condição ser verdadeira.
  - **NÃO (NOT):** inverte o valor lógico.

- **Condições Encadeadas:** permitem múltiplos caminhos de decisão.
  ```pseudocode
  Se (idade < 12) Então
     Escreval("Infantil")
  Senão
     Se (idade < 18) Então
        Escreval("Juvenil")
     Senão
        Escreval("Adulto")
     FimSe
  FimSe

