# Aula 07 - Repetição Condicional
## Tema: Laço ENQUANTO (while)
### Prática: Menu de Opções que só fecha quando o usuário digitar "Sair"

---

## 🎯 Objetivo da Aula
Compreender o funcionamento do **laço ENQUANTO (while)**, ideal para repetições **indefinidas**, quando não sabemos previamente quantas vezes o bloco de código será executado.  
Aplicar esse conceito na criação de menus interativos que permanecem ativos até que o usuário escolha sair.

---

## 💡 Conceito Chave: O Laço ENQUANTO
O laço **ENQUANTO** executa um bloco de código **enquanto** a condição for verdadeira.  
É muito usado em **validação de dados** e **menus interativos**.

**Estrutura:**
```pseudocode
Enquanto (condição) Faça
   // bloco de comandos
FimEnquanto

---

Algoritmo "MenuOpcoes"
Var
   opcao: caractere
Inicio
   opcao <- ""

   Enquanto (opcao <> "Sair") Faça
      Escreval("\n--- MENU ---")
      Escreval("1 - Opção A")
      Escreval("2 - Opção B")
      Escreval("3 - Opção C")
      Escreval("Digite 'Sair' para encerrar.")
      Escreva("Escolha uma opção: ")
      Leia(opcao)

      Se (opcao = "1") Então
         Escreval("Você escolheu a Opção A")
      Senão
         Se (opcao = "2") Então
            Escreval("Você escolheu a Opção B")
         Senão
            Se (opcao = "3") Então
               Escreval("Você escolheu a Opção C")
            Senão
               Se (opcao <> "Sair") Então
                  Escreval("Opção inválida, tente novamente.")
               FimSe
            FimSe
         FimSe
      FimSe
   FimEnquanto

   Escreval("Programa encerrado.")
FimAlgoritmo

- - -

##📝 Exercícios Propostos

**Criar um menu de opções para uma calculadora simples (somar, subtrair, multiplicar, dividir), que só fecha quando o usuário digitar "Sair".**

**Criar um menu de opções para um sistema de cadastro de alunos, com opções de "Cadastrar", "Listar" e "Sair".**

**Criar um menu de opções para um jogo de adivinhação, onde o usuário pode escolher "Jogar", "Ver regras" ou "Sair".**
