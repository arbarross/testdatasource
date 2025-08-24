# **📘 Teste Técnico — Engenheiro de Dados (ETL & Analytics)**

Este repositório contém um banco de dados **SQLite** pré-populado com tabelas de entrada (**SRC**) e uma dimensão de tempo (**dwh_dim_tempo**).  

O candidato deverá usar este banco como **fonte de dados** para criar dimensões derivadas e tabelas fato conforme o enunciado do teste.

---

## **🔹 1. Download do arquivo**

Baixe o arquivo **`pdbdb_investimentos_produto_cdb.sqlite`** deste repositório.  

Você pode:  
- **Clonar o repositório com Git**:
- **Ou clicar em Download** direto no arquivo no GitHub.

---

## **🔹 2. Abrindo o arquivo no DBeaver (recomendado)**

1. Abra o **DBeaver**.  
2. Clique em **Database → New Database Connection**.  
3. Procure por **SQLite** e clique em **Next**.  
4. Em **Database file**, selecione o arquivo **`pdbdb_investimentos_produto_cdb.sqlite`** que você baixou.  
5. Clique em **Finish**.  

Agora você pode navegar pelas tabelas (`src_*` e `dwh_dim_tempo`) e executar queries SQL diretamente.

---

## **🔹 3. Usando o SQLite Web (opção rápida)**

Se preferir rodar o SQLite no navegador:  

1. Instale o pacote **sqlite-web** (precisa do Python instalado):  
   ```bash
   pip install sqlite-web
   ```
2. Rode o comando apontando para o arquivo:  
   ```bash
   sqlite_web pdbdb_investimentos_produto_cdb.sqlite
   ```
3. Abra no navegador o endereço informado (normalmente **http://127.0.0.1:8080**).  

Você verá uma interface web para explorar tabelas e rodar queries.

---

## **🔹 4. Estrutura disponível no banco**

O arquivo já contém as seguintes tabelas com dados:  
- **`src_client_snapshot`**  
- **`src_account_snapshot`**  
- **`src_cdb_produto`**  
- **`src_cdb_ordem`**  
- **`dwh_dim_tempo`**  

👉 Sua tarefa será **criar as dimensões derivadas e a tabela fato** a partir destas tabelas.

---

## **✅ Observações**

- Você pode usar **DBeaver, DB Browser for SQLite, SQLite CLI ou SQLite Web**.  
- O banco é um **arquivo único `.sqlite`**, não precisa de servidor.  
- Lembre-se: suas queries devem ser **idempotentes** (se rodar duas vezes, não pode duplicar dados).  

---

# **📌 Boa sorte no teste! 🚀**
