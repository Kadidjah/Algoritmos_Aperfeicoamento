# Aula 03 - Operadores e Expressões
## Tema: Operadores aritméticos e precedência matemática
### Prática: Calculadora de IMC (Índice de Massa Corporal)

---

## Objetivo
Compreender como utilizar operadores aritméticos (+, -, *, /, %, ^) e aplicar corretamente a ordem de precedência matemática em algoritmos.

---

## Exposição Teórica (15 min)
- **Operadores Aritméticos:**
  - Soma (+)
  - Subtração (-)
  - Multiplicação (*)
  - Divisão (/)
  - Resto da divisão (%)
  - Potência (^)

- **Precedência Matemática:**
  1. Parênteses
  2. Potência
  3. Multiplicação, Divisão e Resto
  4. Soma e Subtração

**Exemplo:**
- `2 + 3 * 4 = 14`  
- `(2 + 3) * 4 = 20`

---

## Mão na Massa (35 min)
### Exercício Prático: Calculadora de IMC

**Fórmula:**

IMC = peso * altura


### Pseudocódigo (Visualg)
```pseudocode
Algoritmo "CalculadoraIMC"
Var
   peso: real
   altura: real
   imc: real
Inicio
   Escreva("Digite seu peso (kg): ")
   Leia(peso)
   Escreva("Digite sua altura (m): ")
   Leia(altura)

   imc <- peso / (altura ^ 2)

   Escreval("Seu IMC é: ", imc:2:2)
FimAlgoritmo
