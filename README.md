# 🚗 Projeto Carros - Banco de Dados MySQL

![GitHub Repo Size](https://img.shields.io/github/repo-size/MrRobii/meu-projeto-mysql?style=flat-square)
![GitHub Language](https://img.shields.io/github/languages/top/MrRobii/meu-projeto-mysql?style=flat-square)
![GitHub License](https://img.shields.io/github/license/MrRobii/meu-projeto-mysql?style=flat-square)

Este repositório contém o banco de dados **carros.sql**, com tabelas e dados de exemplo sobre carros.

---

## 🗂 Estrutura do Banco

| Tabela      | Descrição                                  |
|------------|-------------------------------------------|
| `Carros`   | Informações sobre modelos, marcas e anos |

---

## ⚡ Como importar o banco MySQL

### 1️⃣ Usando MySQL Workbench (GUI)

1. Abra o **MySQL Workbench**.
2. Conecte-se ao seu servidor MySQL.
3. Vá em **Server → Data Import**.
4. Escolha **Import from Self-Contained File** e selecione [`carros.sql`](carros.sql).
5. Clique em **Start Import**.
6. O banco será criado e estará pronto para uso.

### 2️⃣ Usando Linha de Comando (Terminal / CMD)

```bash
mysql -u <usuario> -p <nome_do_banco> < carros.sql

Substitua <usuario> pelo seu usuário MySQL.

Substitua <nome_do_banco> pelo nome que deseja para o banco.

Digite sua senha quando solicitado.

📝 Exemplos de Consultas SQL

-- Selecionar todos os carros
SELECT * FROM Carros;

-- Filtrar carros por marca
SELECT * FROM Carros WHERE marca = 'Toyota';

-- Contar quantos carros existem por ano
SELECT ano, COUNT(*) as total FROM Carros GROUP BY ano;
