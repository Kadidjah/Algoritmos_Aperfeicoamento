# Calculadora de IMC com classificação

peso = float(input("Digite seu peso (kg): "))
altura = float(input("Digite sua altura (m): "))

imc = peso / (altura ** 2)

print(f"Seu IMC é: {imc:.2f}")

# Classificação segundo OMS
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

