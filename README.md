# Prova-Banco-de-Dados

## Descrição
Este repositório têm minha resolução da prova prática da disciplina de Banco de Dados, com foco no MongoDB, integrado à linguagem de
programação Python. A prova é para avaliar a capacidade do aluno de configurar o ambiente
de banco de dados, manipular coleções de dados no formato JSON e implementar
operações essenciais de CRUD (Create, Read, Update, Delete) usando scripts em
Python.

## Requisitos
- Python +3.13.x
- MongoDB Compass se escolher formato local ou Conta no MongoDB Atlas(nuvem). Usei o Atlas nessa entrega.

## Instalação
1. Clone o repositório
2. Crie um ambiente virtual: `python -m venv venv`
3. Ative o ambiente virtual
4. Instale as dependências: `pip install -r requirements.txt`

## Configuração
1. Copie `.env.example` para `.env`
2. Preencha as variáveis com seus dados do MongoDB Atlas ou do MongoDB Compass

## Como executar
1. Execute `pymongo_get_connection_eventos.py` para testar a conexão
2. Execute `pymongo_crud_eventos.py` para rodar as operações de CRUD

## Funcionalidades (CRUD)
- Create: Inserir novos documentos na coleção.
- Read: Consultar e listar documentos da coleção
- Update: Modificar dados de documentos existentes.
- Delete: Remover documentos da coleção.

### Consulta Avançada
- Criação de uma função especial que realiza uma consulta utilizando
filtros com operadores numéricos (ex: $gt, $lt, $gte, $lte) ou um pipeline de
agregação (aggregate), demonstrando domínio sobre consultas complexas no
MongoDB. Escolhi fazer uma pipeline de agregação.

## Estrutura do repositório
- **.env.example:** É um "molde" que mostra as variáveis de ambiente necessárias (sem credenciais reais).
- **.gitignore:** Arquivo que diz ao Git para ignorar o .env e pastas temporárias.
- **README.md:** documento explicando: o que ele faz, como configurar o ambiente, como rodar, assim por diante.
- **eventos.json:** arquivo .json oferecido pelo professor, com dados fictícios de eventos.
- **participantes.json:** arquivo .json oferecido pelo professor, com dados fictícios sobre os participantes dos eventos.
- **pymongo_crud_eventos.py:** script com funções de inserção, busca, atualização e deleção além de uma consulta avançada.
- **pymongo_get_connection_eventos.py:** script focado em estabelecer a conexão ao banco de dados(local ou Atlas).
- **requirements.txt:** arquivo com as dependências(ex: pymongo).
