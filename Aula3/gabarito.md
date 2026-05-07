# Calculadora de IMC com classificação

# Aula 03 - Operadores e Expressões
## Calculadora de IMC em Visualg

---

### Código Completo

```pseudocode
Algoritmo "CalculadoraIMC"
Var
   peso: real
   altura: real
   imc: real
Inicio
   // Entrada de dados
   Escreva("Digite seu peso (kg): ")
   Leia(peso)
   Escreva("Digite sua altura (m): ")
   Leia(altura)

   // Processamento
   imc <- peso / (altura ^ 2)

   // Saída do resultado
   Escreval("Seu IMC é: ", imc:2:2)

   // Classificação segundo a OMS
   Se (imc < 18.5) Então
      Escreval("Classificação: Abaixo do peso")
   Senão
      Se (imc < 25) Então
         Escreval("Classificação: Peso normal")
      Senão
         Se (imc < 30) Então
            Escreval("Classificação: Sobrepeso")
         Senão
            Escreval("Classificação: Obesidade")
         FimSe
      FimSe
   FimSe
FimAlgoritmo
