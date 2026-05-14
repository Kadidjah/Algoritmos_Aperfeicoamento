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

## Visualg

# Aula 05 - Tomada de Decisão II
## Algoritmo em Visualg: Classificação de Atletas por Idade

---

### Código Completo
```pseudocode
Algoritmo "ClassificacaoAtletasCompleta"
Var
   idade: inteiro
Inicio
   Escreva("Digite a idade do atleta: ")
   Leia(idade)

   Se (idade < 12) Então
      Escreval("Categoria: Infantil")
   Senão
      Se (idade < 18) Então
         Escreval("Categoria: Juvenil")
      Senão
         Se (idade < 30) Então
            Escreval("Categoria: Adulto Jovem")
         Senão
            Se (idade < 45) Então
               Escreval("Categoria: Adulto Intermediário")
            Senão
               Se (idade < 60) Então
                  Escreval("Categoria: Adulto Sênior")
               Senão
                  Escreval("Categoria: Master")
               FimSe
            FimSe
         FimSe
      FimSe
   FimSe
FimAlgoritmo

## Explicação

Variável: idade (inteiro).

Entrada: o usuário fornece a idade.

Processamento: decisão encadeada com base em faixas etárias.

Saída: categoria do atleta, incluindo subcategorias dentro de Adulto.

