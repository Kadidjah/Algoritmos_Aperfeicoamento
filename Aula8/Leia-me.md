# Aula 08 - Vetores (Arrays)
## Tema: Estruturas Indexadas
### Prática: Armazenamento e manipulação de múltiplos dados

---

## 🎯 Objetivo da Aula
Capacitar o aluno a armazenar e manipular múltiplos dados de um mesmo tipo sob um único identificador, utilizando **estruturas indexadas (vetores/arrays)**.

---

## 💡 Conceito Chave: Vetores
- Um **vetor** é uma estrutura que armazena vários valores do mesmo tipo.  
- Cada valor ocupa uma **posição (índice)** dentro do vetor.  
- Os índices geralmente começam em **0** (Python) ou **1** (Visualg).  

**Exemplo de vetor com 5 elementos:**

---

## 💻 Exemplo Prático: Notas de Alunos

### Código em Python
```python
# Aula 08 - Vetores (Arrays)
# Armazenamento de notas de alunos

notas = []  # vetor vazio

# Entrada de dados
for i in range(5):
    nota = float(input(f"Digite a nota {i+1}: "))
    notas.append(nota)

---

## 🔍 Análise do Fluxo de Execução

1. **Criação do vetor:**  
   `notas = []` inicia vazio.

2. **Entrada:**  
   O laço `for` coleta 5 notas e adiciona ao vetor com `.append()`.

3. **Processamento:**  
   Usamos `sum(notas)` para somar e `len(notas)` para contar.

4. **Saída:**  
   Exibimos todas as notas e a média final.

# Processamento
media = sum(notas) / len(notas)

# Saída

---

## 🚀 Desafio Extra

👉 Expanda o programa para identificar a maior e a menor nota da turma.

### Código em Python (Desafio Extra)

```python
notas = []

# Entrada de dados
for i in range(5):
    nota = float(input(f"Digite a {i+1}ª nota: "))
    notas.append(nota)

# Processamento
media = sum(notas) / len(notas)
maior_nota = max(notas)
menor_nota = min(notas)

# Saída
print("\nNotas digitadas:", notas)
print(f"Média da turma: {media:.2f}")
print(f"Maior nota: {maior_nota}")
print(f"Menor nota: {menor_nota}")
print("\nNotas digitadas:", notas)
print(f"Média da turma: {media:.2f}")

---

## 📝 Exercícios Propostos

1. Criar um vetor com 10 números inteiros e exibir apenas os pares.

2. Criar um vetor com 8 nomes e exibir apenas os que começam com a letra A.

3. Criar um vetor com 12 temperaturas e calcular a média anual, mostrando também a maior e a menor temperatura.

---

## 📚 Materiais de Apoio

- **Slides:** Aula 8 - Arrays  
- **Ferramenta:** Python (Google Colab)
- **Referência:** Algoritmos Estruturados – Harry Farrer.
