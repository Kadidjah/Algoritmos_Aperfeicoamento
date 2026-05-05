# Aula 02 - Memória e Dados
## Sistema de Cadastro para Biblioteca (Python)

### Objetivo
Compreender como o computador guarda informações utilizando **variáveis, constantes e tipos de dados**.  
Aplicar esses conceitos em um sistema simples de cadastro de livros.

---

### Código em Python

```python
# Aula 02 - Memória e Dados
# Sistema de Cadastro para Biblioteca

# Entrada de dados
titulo_livro = input("Digite o título do livro: ")
autor = input("Digite o autor: ")
ano_publicacao = int(input("Digite o ano de publicação: "))
disponivel = input("O livro está disponível? (sim/não): ")

# Processamento
# Convertendo a resposta para um valor lógico
if disponivel.lower() == "sim":
    disponivel = True
else:
    disponivel = False

# Saída organizada
print("\nCadastro realizado com sucesso!")
print(f"Título: {titulo_livro}")
print(f"Autor: {autor}")
print(f"Ano: {ano_publicacao}")
print(f"Disponível: {disponivel}")

## Explicação

- **Variáveis:** armazenam dados que podem mudar durante a execução (`titulo_livro`, `autor`, `ano_publicacao`, `disponivel`).

- **Tipos de dados:**
  - `str` → texto (strings)
  - `int` → números inteiros
  - `bool` → valores lógicos (`True` / `False`)

- **Entrada:** `input()` sempre retorna texto, por isso usamos `int()` para converter o ano.

- **Processamento:** transformamos a resposta `"sim/não"` em um valor lógico.

- **Saída:** usamos `f-strings` para organizar a frase final.

---

## Desafio Extra

Expanda o programa para cadastrar **dois livros** e exibir ambos ao final.

👉 Esse exercício reforça o uso de variáveis e prepara para o conteúdo de **listas (arrays)** na **Aula 08**.
