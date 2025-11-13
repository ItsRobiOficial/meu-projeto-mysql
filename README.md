# 🚗 Projeto Carros — Banco de Dados MySQL  

![GitHub Repo Size](https://img.shields.io/github/repo-size/MrRobii/meu-projeto-mysql?style=flat-square)
![GitHub Language](https://img.shields.io/github/languages/top/MrRobii/meu-projeto-mysql?style=flat-square)
![GitHub License](https://img.shields.io/github/license/MrRobii/meu-projeto-mysql?style=flat-square)

Este repositório contém o banco de dados **`carros.sql`**, com tabelas e dados de exemplo sobre modelos, marcas e anos de veículos.  
Ideal para praticar **consultas SQL**, **modelagem de dados** e **operações CRUD**.

---

## 🗂 Estrutura do Banco de Dados

| Tabela  | Descrição |
|----------|------------|
| `Carros` | Contém informações sobre modelos, marcas, anos e preços. |

---

## ⚙️ Como Importar o Banco de Dados

### 🔹 Opção 1 — Usando MySQL Workbench (Interface Gráfica)

1. Abra o **MySQL Workbench**.  
2. Conecte-se ao seu servidor MySQL.  
3. Vá em **Server → Data Import**.  
4. Escolha **Import from Self-Contained File** e selecione [`carros.sql`](carros.sql).  
5. Clique em **Start Import**.  
6. O banco será criado automaticamente e estará pronto para uso.  

---

### 🔹 Opção 2 — Usando Linha de Comando (Terminal / CMD)

```bash
mysql -u <usuario> -p <nome_do_banco> < carros.sql
```

🔧 Substitua <usuario> pelo seu usuário MySQL e <nome_do_banco> pelo nome desejado.
Depois, digite sua senha quando solicitado.

-- Selecionar todos os carros
SELECT * FROM Carros;

-- Filtrar carros por marca
SELECT * FROM Carros WHERE marca = 'Toyota';

-- Contar quantos carros existem por ano
SELECT ano, COUNT(*) AS total FROM Carros GROUP BY ano;

---

🧠 Exemplos de Consultas SQL

-- Selecionar todos os carros
SELECT * FROM Carros;

-- Filtrar carros por marca
SELECT * FROM Carros WHERE marca = 'Toyota';

-- Contar quantos carros existem por ano
SELECT ano, COUNT(*) AS total FROM Carros GROUP BY ano;

---

💡 Objetivo do Projeto

Este projeto foi criado para:
Praticar comandos SQL (SELECT, INSERT, UPDATE, DELETE).
Aprender estruturação de tabelas relacionais.
Simular cenários reais de análise de dados automotivos.

---

⭐ Se este projeto te ajudou, deixe uma estrela e contribua!


