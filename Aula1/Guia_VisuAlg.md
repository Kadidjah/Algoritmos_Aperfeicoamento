# Guia de Utilização Básica: VisuALG

Este guia fundamental foi desenvolvido para orientar seus primeiros passos no VisuALG, utilizando como base a metodologia pedagógica aplicada no IFSC (Instituto Federal de Santa Catarina) - Campus Lages, sob a orientação do Prof. Vilson Heck Junior.

Nosso objetivo é transformar a lógica abstrata em ferramentas práticas para a criação de seus primeiros programas.

---

# 1. Introdução ao VisuALG: O Ponto de Partida

O VisuALG, concebido pelo Prof. Cláudio Morgado de Souza (Apoio Informática), é um software de auxílio ao ensino de programação que permite ao aluno focar totalmente na lógica, sem as complexidades sintáticas de linguagens comerciais.

Ele utiliza o **Português Estruturado (pseudocódigo)** para criar uma ponte suave entre o pensamento humano e a execução computacional.

## Principais Vantagens do VisuALG

- **Simplicidade Técnica:** Muito mais acessível que linguagens como C ou Java para quem está começando.
- **Português Estruturado:** Elimina a barreira do idioma, permitindo que você escreva comandos em sua língua nativa.
- **Ambiente de Aprendizado:** Projetado especificamente para fins pedagógicos, facilitando a visualização do fluxo de dados e a depuração de erros.

Compreender a finalidade desta ferramenta é o primeiro passo; o segundo é aprender como organizar suas ideias dentro da estrutura que o software exige.

---

# 2. A Anatomia do Código: Estrutura Básica

Para que o VisuALG entenda suas instruções, o código deve seguir uma estrutura padronizada, dividida em blocos de responsabilidade.

Pense nisso como o **esqueleto** do seu programa.

```pascal
algoritmo "nome_do_algoritmo"

// Função : Descrição clara da utilidade do programa
// Autor   : Seu Nome
// Data    : 22/05/2024

// Seção de Declarações de Variáveis
var

inicio

   // Seção de Comandos (aqui o código ganha vida)

fimalgoritmo
```

## Entendendo as Seções

| Seção | Finalidade |
|---------|-----------|
| `algoritmo` | Identifica o nome do projeto. |
| `var` | Espaço de preparação onde declaramos as variáveis. |
| `inicio` | Marca o início da execução do programa. |
| `fimalgoritmo` | Marca o fim da execução do programa. |
| `// comentário` | Anotações ignoradas pelo VisuALG. |

### Comentários

Os comentários são essenciais para a organização do código.

Tudo o que vier após `//` será ignorado pelo VisuALG, permitindo que você documente sua lógica.

---

# 3. Variáveis: Declarando e Atribuindo Valores

As variáveis são espaços na memória do computador destinados a armazenar informações.

Antes de utilizar um dado, é necessário declarar:

- Nome da variável
- Tipo da variável

## Tipos de Dados Fundamentais

| Tipo de Dado | Exemplo |
|-------------|----------|
| `inteiro` | 10, -5, 0 |
| `real` | 10.5, 3.14 |
| `logico` | verdadeiro, falso |
| `caractere` | "Olá", "A", "123" |

## Declaração vs. Atribuição

### Declaração

Realizada na seção `var`.

```pascal
var
   idade : inteiro
   nome  : caractere
```

### Atribuição

Realizada na seção `inicio`.

```pascal
idade <- 20
nome <- "Maria"
```

### Pro-Tip

É possível declarar várias variáveis do mesmo tipo em uma única linha:

```pascal
var
   x, y, z : real
```

### Dica de Sintaxe

O VisuALG é, em geral, **case-insensitive**.

Portanto:

```pascal
n : inteiro

N <- 10
```

funciona normalmente.

Mesmo assim, manter consistência é uma boa prática.

---

# 4. Comandos de Saída: Mostrando Resultados

Os comandos de saída exibem informações para o usuário.

## `escreva`

Exibe informações sem quebrar a linha.

```pascal
escreva("Olá ")
escreva("Mundo")
```

Saída:

```text
Olá Mundo
```

## `escreval`

Exibe informações e pula para a próxima linha.

```pascal
escreval("Olá")
escreval("Mundo")
```

Saída:

```text
Olá
Mundo
```

## Exemplo Prático

```pascal
inicio

   escreva("Resultado parcial: ")
   escreval(10)

   escreval("Fim do processo.")

fimalgoritmo
```

---

# 5. Comandos de Entrada: Capturando Dados

O comando `leia()` permite que o usuário forneça informações ao programa.

## Sintaxe

```pascal
leia(variavel)
```

## Exemplo

```pascal
var
   nome : caractere

inicio

   escreva("Digite seu nome: ")
   leia(nome)

   escreval("Olá ", nome)

fimalgoritmo
```

### O "So What?" Pedagógico

Imagine que o comando `leia` é a ponte entre o cérebro do usuário e a memória do computador.

Sem ele, o programa sempre executaria os mesmos cálculos.

Com ele, o algoritmo se torna dinâmico e interativo.

---

# 6. Operadores Aritméticos e a Lógica do Cálculo

## Tabela de Operadores

| Operação | Operador | Observação |
|-----------|-----------|-----------|
| Adição | `+` | Soma valores |
| Subtração | `-` | Subtrai valores |
| Multiplicação | `*` | Multiplica valores |
| Divisão | `/` | Retorna valor real |
| Divisão Inteira | `\` | Descarta o resto |
| Exponenciação | `^` | Potência |
| Função Potência | `Exp(b,e)` | Base e expoente |
| Módulo | `%` | Resto da divisão |
| Raiz Quadrada | `raizq()` | Calcula a raiz |

## Exemplos

```pascal
5 / 2
```

Resultado:

```text
2.5
```

```pascal
5 \ 2
```

Resultado:

```text
2
```

```pascal
5 % 2
```

Resultado:

```text
1
```

```pascal
2 ^ 3
```

Resultado:

```text
8
```

```pascal
raizq(25)
```

Resultado:

```text
5
```

---

## Ordem de Precedência

O VisuALG segue a seguinte hierarquia:

1. Parênteses `()`
2. Exponenciação `^` ou `Exp()`
3. Multiplicação e divisões `*`, `/`, `\`, `%`
4. Adição e subtração `+`, `-`

### Exemplo 1

```pascal
(2 + 2) / 2
```

Resultado:

```text
2
```

### Exemplo 2

```pascal
2 + 2 / 2
```

Resultado:

```text
3
```

### O Poder dos Parênteses

Use parênteses sempre que desejar forçar uma operação a acontecer antes das demais.

---

# 7. Desafios Práticos: Consolidação do Conhecimento

Aplique os conceitos aprendidos nos exercícios abaixo.

---

## Desafio 1: Mensagens e Formatação

Crie um algoritmo que:

1. Solicite o nome do usuário.
2. Exiba:

```text
Olá, [Nome]!
Seja bem-vindo ao VisuALG!
```

### Dica de Mestre

Utilize:

- `escreva` para o convite de digitação.
- `escreval` para garantir a quebra de linha.

---

## Desafio 2: Captura de Caractere

Crie um programa que:

1. Leia um único caractere.
2. Exiba esse caractere em uma frase personalizada.

Exemplo:

```text
Você informou o sexo: M
```

### Dica de Mestre

Variáveis do tipo `caractere` não realizam operações matemáticas.

Sempre utilize aspas ao atribuir valores textuais:

```pascal
sexo <- "M"
```

---

## Desafio 3: Cálculos Matemáticos

Implemente uma das opções abaixo.

### Opção 1: Média Aritmética

Leia três números e calcule:

```text
média = (n1 + n2 + n3) / 3
```

### Opção 2: Área do Círculo

Leia o raio `R` e calcule:

```text
A = π × R²
```

Considere:

```text
π = 3.14
```

### Dica de Mestre

Para obter resultados com casas decimais:

```pascal
var
   n1, n2, n3, media : real
```

Não esqueça dos parênteses:

```pascal
media <- (n1 + n2 + n3) / 3
```

---

# Conclusão

Dominar os comandos básicos do VisuALG é o alicerce para construir algoritmos cada vez mais inteligentes e poderosos.

Pratique constantemente os conceitos apresentados neste guia e avance gradualmente para estruturas de decisão, repetição e modularização.

**Bom trabalho e bons estudos!**
