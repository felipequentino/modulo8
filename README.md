# Lab 01: Python & C#

## Objetivo
Criar seus primeiros programas em Back-end, entendendo na prática a diferença entre uma linguagem dinâmica (Python) e uma estática (C#).

---

## PARTE 1

Siga os passos abaixo no seu computador.  
Lembre-se: o terminal será sua principal ferramenta neste laboratório.

---

## Passo 0: Check-up

1. Abra o VS Code.
2. Abra o Terminal:
   - Atalho: Ctrl + '
   - Ou menu: Terminal > New Terminal
3. Verifique se as ferramentas estão instaladas:

```bash
python --version
dotnet --version
````

Se aparecerem números de versão, você está pronto para continuar.

---

## Passo 1: Organização

1. Crie uma pasta na Área de Trabalho chamada `Modulo8`.
2. Dentro dela, crie outra pasta chamada `Dia01`.
3. Abra a pasta `Dia01` no VS Code:

   * File > Open Folder

---

## Exercício 1: Olá Mundo Comparativo

Vamos observar como cada linguagem inicia um projeto simples.

---

### Python (Execução Direta)

1. Crie um arquivo chamado `hello.py`.
2. Escreva o código:

```python
print("Olá, Turma! Este é o Python.")
nome = "SeuNome"
print(f"Bem-vindo ao Backend, {nome}")
```

3. Execute no terminal:

```bash
python hello.py
```

---

### C# (Projeto Estruturado)

1. No terminal, crie o projeto:

```bash
dotnet new console -n HelloCSharp
```

2. Entre na pasta criada:

```bash
cd HelloCSharp
```

3. Abra o arquivo `Program.cs`, apague todo o conteúdo e substitua por:

```csharp
Console.WriteLine("Olá, Turma! Este é o C#.");
string nome = "SeuNome";
Console.WriteLine($"Bem-vindo ao Backend, {nome}");
```

4. Execute:

```bash
dotnet run
```

---

## Exercício 2: O Crachá Digital

O RH precisa de um sistema para cadastrar novos desenvolvedores.

### Requisitos

O programa deve:

* Perguntar o nome (texto)
* Perguntar a idade (inteiro)
* Perguntar o salário pretendido (decimal)
* Perguntar se já tem experiência
* Exibir todas as informações formatadas ao final

Observação para C#:
`Console.ReadLine()` sempre retorna texto. Use `int.Parse()` ou `double.Parse()` para conversão.

---

## Desafio Final: Calculadora de 13º Salário

Crie um novo programa em Python e depois em C#.

### Regras

1. O usuário informa o salário mensal bruto.
2. O sistema calcula:

   * Salário anual bruto (salário * 13)
   * Desconto fictício de 10%
   * Salário líquido final
3. Exibir:

   * Salário anual bruto
   * Valor do desconto
   * Salário líquido
