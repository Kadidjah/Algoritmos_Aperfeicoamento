# Aula 06 - Repetição Controlada
## Tema: Laço PARA (for)
### Prática: Tabuada Personalizada

---

## Objetivo da Aula
Compreender o funcionamento do **laço PARA (for)**, ideal para repetições com limites fixos e contagens predeterminadas.

---

## 💡 Conceito Chave: O Laço PARA
O laço **PARA** é utilizado quando já sabemos exatamente quantas vezes o bloco de código deve ser executado.  
Ele agrupa três estruturas em uma única linha:

1. **Inicialização:** Define o valor inicial do contador.  
2. **Condição:** Determina até quando o laço deve rodar.  
3. **Incremento:** Altera o valor do contador a cada repetição.  

---

## 💻 Exemplo Prático: Tabuada Personalizada
O programa pede um número ao usuário e gera a tabuada de 1 a 10 para esse número.

---

### Código em Visualg
```pseudocode
Algoritmo "TabuadaPersonalizada"
Var
   numero, resultado, contador: inteiro
Inicio
   Escreva("Digite um número para ver a tabuada: ")
   Leia(numero)

   Escreval("\n--- Tabuada do ", numero, " ---")

   Para contador <- 1 Ate 10 Faca
      resultado <- numero * contador
      Escreval(numero, " x ", contador, " = ", resultado)
   FimPara
FimAlgoritmo
