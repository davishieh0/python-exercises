# python-exercises
# Exercícios Python: Listas e Loops de Repetição

## Exercício 1: Lista Básica - Frutas Favoritas

**Enunciado:** Crie uma lista com 5 frutas diferentes e imprima cada fruta em uma linha separada.

**Código esperado:**
```python
frutas = ["maçã", "banana", "laranja", "uva", "morango"]
for fruta in frutas:
    print(fruta)
```

**Stdout esperado:**
```
maçã
banana
laranja
uva
morango
```

---

## Exercício 2: Lista com Números - Tabuada do 5

**Enunciado:** Crie uma lista com os números de 1 a 10 e imprima a tabuada do 5 para cada número.

**Código esperado:**
```python
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for num in numeros:
    resultado = num * 5
    print(f"5 x {num} = {resultado}")
```

**Stdout esperado:**
```
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

---

## Exercício 3: Lista com Condicionais - Números Pares

**Enunciado:** Crie uma lista com números de 1 a 20 e imprima apenas os números pares, indicando que são pares.

**Código esperado:**
```python
numeros = list(range(1, 21))
for num in numeros:
    if num % 2 == 0:
        print(f"{num} é par")
```

**Stdout esperado:**
```
2 é par
4 é par
6 é par
8 é par
10 é par
12 é par
14 é par
16 é par
18 é par
20 é par
```

---

## Exercício 4: Lista de Notas - Aprovados e Reprovados

**Enunciado:** Crie uma lista com 8 notas de alunos (valores entre 0 e 10) e imprima o status de cada nota (Aprovado se >= 7, Reprovado se < 7).

**Código esperado:**
```python
notas = [8.5, 6.0, 7.5, 4.5, 9.0, 5.5, 8.0, 7.0]
for i, nota in enumerate(notas):
    if nota >= 7:
        status = "Aprovado"
    else:
        status = "Reprovado"
    print(f"Aluno {i+1}: Nota {nota} - {status}")
```

**Stdout esperado:**
```
Aluno 1: Nota 8.5 - Aprovado
Aluno 2: Nota 6.0 - Reprovado
Aluno 3: Nota 7.5 - Aprovado
Aluno 4: Nota 4.5 - Reprovado
Aluno 5: Nota 9.0 - Aprovado
Aluno 6: Nota 5.5 - Reprovado
Aluno 7: Nota 8.0 - Aprovado
Aluno 8: Nota 7.0 - Aprovado
```

---

## Exercício 5: DESAFIO - Sistema de Inventário de Loja

**Enunciado:** Crie um sistema de inventário para uma loja que:
1. Tenha uma lista de produtos (nome, preço, quantidade)
2. Calcule o valor total do estoque
3. Identifique produtos em falta (quantidade = 0)
4. Identifique produtos com estoque baixo (quantidade <= 5)
5. Encontre o produto mais caro e o mais barato
6. Gere um relatório completo

**Dados para usar:**
```python
produtos = [
    ["Notebook", 2500.00, 3],
    ["Mouse", 50.00, 0],
    ["Teclado", 150.00, 8],
    ["Monitor", 800.00, 2],
    ["Headset", 200.00, 5],
    ["Webcam", 300.00, 0],
    ["Impressora", 450.00, 1],
    ["Tablet", 1200.00, 4]
]
```

**Dicas para resolução:**
- Use listas aninhadas para armazenar [nome, preço, quantidade]
- Utilize loops para percorrer os produtos
- Implemente condicionais para categorizar produtos
- Use acumuladores para somar valores
- Aplique formatação adequada para o relatório

**Stdout esperado:**
```
=== RELATÓRIO DE INVENTÁRIO ===

Valor total do estoque: R$ 14050.00
Produto mais caro: Notebook (R$ 2500.00)
Produto mais barato: Mouse (R$ 50.00)

--- PRODUTOS SEM ESTOQUE ---
⚠️  Mouse
⚠️  Webcam

--- PRODUTOS COM ESTOQUE BAIXO (≤5) ---
⚠️  Monitor
⚠️  Headset
⚠️  Impressora
⚠️  Tablet

--- DETALHAMENTO POR PRODUTO ---
Notebook: 3 unidades | R$ 2500.00 cada | Total: R$ 7500.00 | Status: OK
Mouse: 0 unidades | R$ 50.00 cada | Total: R$ 0.00 | Status: SEM ESTOQUE
Teclado: 8 unidades | R$ 150.00 cada | Total: R$ 1200.00 | Status: OK
Monitor: 2 unidades | R$ 800.00 cada | Total: R$ 1600.00 | Status: ESTOQUE BAIXO
Headset: 5 unidades | R$ 200.00 cada | Total: R$ 1000.00 | Status: ESTOQUE BAIXO
Webcam: 0 unidades | R$ 300.00 cada | Total: R$ 0.00 | Status: SEM ESTOQUE
Impressora: 1 unidades | R$ 450.00 cada | Total: R$ 450.00 | Status: ESTOQUE BAIXO
Tablet: 4 unidades | R$ 1200.00 cada | Total: R$ 4800.00 | Status: ESTOQUE BAIXO
```

---

## Dicas para Resolução

1. **Comece simples**: Teste cada parte do código separadamente
2. **Use print() para debug**: Imprima variáveis para entender o fluxo
3. **Planeje antes de codificar**: Escreva os passos em português primeiro
4. **Teste com dados diferentes**: Mude os valores das listas para testar
5. **Pratique a sintaxe**: for, if, enumerate, range, len()

## Próximos Passos

Após dominar esses exercícios, você estará preparado para:
- Funções com listas
- List comprehensions
- Dicionários e loops
- Manipulação de arquivos
- Estruturas de dados mais complexas
