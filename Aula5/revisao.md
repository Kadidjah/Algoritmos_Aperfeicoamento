# Curso de Algoritmos e Lógica de Programação
## Material de Apoio – Gabaritos e Exercícios

---

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

titulo_livro = input("Digite o título do livro: ")
autor = input("Digite o autor: ")
ano_publicacao = int(input("Digite o ano de publicação: "))
disponivel = input("O livro está disponível? (sim/não): ")

if disponivel.lower() == "sim":
    disponivel = True
else:
    disponivel = False

print("\nCadastro realizado com sucesso!")
print(f"Título: {titulo_livro}")
print(f"Autor: {autor}")
print(f"Ano: {ano_publicacao}")
print(f"Disponível: {disponivel}")

