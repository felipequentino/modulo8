# Lab 01: Python & C#

## Objetivo
Criar seus primeiros programas em Back-end, entendendo na prática a diferença entre uma linguagem dinâmica (Python) e uma estática (C#).

---

## Configuração do Ambiente (Windows)

Antes de começar, você precisa preparar seu computador. Siga os passos abaixo para instalar as ferramentas necessárias.

### 1. Editor de Código (VS Code)
Se você ainda não tem o VS Code:
1. Acesse: [code.visualstudio.com](https://code.visualstudio.com/)
2. Clique em **Download for Windows**.
3. Instale com as opções padrão (apenas vá clicando em "Próximo").

### 2. Instalando o Python
1. Acesse: [python.org/downloads](https://www.python.org/downloads/)
2. Clique no botão amarelo **Download Python 3.x.x**.
3. **⚠️ IMPORTANTE:** Ao abrir o instalador, marque a caixinha:
   **[x] Add python.exe to PATH** (Adicionar Python ao PATH).
4. Clique em **Install Now**.

### 3. Instalando o C# (.NET SDK)
Para programar em C#, precisamos do **.NET SDK** (Software Development Kit).
1. Acesse: [dotnet.microsoft.com/download](https://dotnet.microsoft.com/download)
2. Procure pela aba **.NET 8.0** (ou a versão mais recente "LTS").
3. Clique no botão **Download .NET SDK x64** (para Windows).
4. Abra o instalador e clique em **Install**.

---

## PARTE 1: Mão na Massa

Siga os passos abaixo no seu computador.  
Lembre-se: o terminal será sua principal ferramenta neste laboratório.

---

## Passo 0: Check-up

Agora vamos verificar se a instalação funcionou.

1. Abra o VS Code.
2. Abra o Terminal:
   - Atalho: `Ctrl + '` (aspas simples) ou `Ctrl + J`
   - Ou menu: **Terminal > New Terminal**
3. Digite os comandos abaixo (um por vez) e aperte Enter:

```bash
python --version
dotnet --version

```

Se aparecerem números de versão (ex: `Python 3.12.0` e `8.0.100`), você está pronto para continuar!

---

## Passo 1: Organização

1. Crie uma pasta na Área de Trabalho chamada `Modulo8`.
2. Dentro dela, crie outra pasta chamada `Dia01`.
3. Abra a pasta `Dia01` no VS Code:
* **File > Open Folder** (Arquivo > Abrir Pasta) e selecione a pasta `Dia01`.



---

## Exercício 1: Olá Mundo Comparativo

Vamos observar como cada linguagem inicia um projeto simples.

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

**Dica para C#:**
`Console.ReadLine()` sempre retorna texto (string). Você precisará converter:

* Para inteiro: `int.Parse(Console.ReadLine())`
* Para decimal: `double.Parse(Console.ReadLine())` ou `decimal.Parse(...)`

---

## Desafio Final: Calculadora de 13º Salário

Crie um novo programa em Python e depois em C#.

### Regras

1. O usuário informa o salário mensal bruto.
2. O sistema calcula:
* **Salário anual bruto** (salário * 13)
* **Desconto fictício de 10%** sobre o total anual
* **Salário líquido final** (Anual - Desconto)


3. Exibir:
* Salário anual bruto
* Valor do desconto
* Salário líquido
