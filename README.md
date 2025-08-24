📘 README — Teste Técnico Engenheiro de Dados (ETL & Analytics)

Este repositório contém um banco de dados SQLite pré-populado com tabelas de entrada (SRC) e uma dimensão de tempo (dwh_dim_tempo).

O candidato deverá usar este banco como fonte de dados para criar dimensões derivadas e tabelas fato conforme o enunciado do teste.

🔹 1. Download do arquivo

Baixe o arquivo etl_cdb_broker_test_v3_reduced.sqlite deste repositório.
Você pode:

Clonar o repositório com Git:

git clone https://github.com/<seu-repo>/teste-etl.git
cd teste-etl


Ou clicar em Download direto no arquivo no GitHub.

🔹 2. Abrindo o arquivo no DBeaver (recomendado)

Abra o DBeaver.

Clique em Database → New Database Connection.

Procure por SQLite e clique em Next.

Em Database file, selecione o arquivo etl_cdb_broker_test_v3_reduced.sqlite que você baixou.

Clique em Finish.

Agora você pode navegar pelas tabelas (src_* e dwh_dim_tempo) e executar queries SQL diretamente.

🔹 3. Usando o SQLite Web (opção rápida)

Se preferir rodar o SQLite em navegador:

Instale o pacote sqlite-web (precisa do Python instalado):

pip install sqlite-web


Rode o comando apontando para o arquivo:

sqlite_web etl_cdb_broker_test_v3_reduced.sqlite


Abra no navegador o endereço informado (normalmente http://127.0.0.1:8080).

Você verá uma interface web para explorar tabelas e rodar queries.

🔹 4. Estrutura disponível no banco

O arquivo contém as seguintes tabelas já carregadas com dados:

src_client_snapshot

src_account_snapshot

src_cdb_produto

src_cdb_ordem

dwh_dim_tempo

👉 Sua tarefa será criar as dimensões derivadas e a tabela fato a partir destas tabelas.

✅ Observações

Você pode usar DBeaver, DB Browser for SQLite, SQLite CLI ou SQLite Web.

O banco é um arquivo único .sqlite, não precisa de servidor.

Lembre-se de garantir que suas queries sejam idempotentes (se rodar duas vezes, não deve duplicar dados).

📌 Boa sorte no teste! 🚀
