# extracao_twitter_airflow

# anotações

  ## site alternativa para api para o curso.
  https://labdados.com/.

    Admin/Connections
    Add
    Connection Id = twitter_default
    Connection Type = Http
    Host = https://labdados.com
    Extra = {"Authorization": "Bearer XXXXXXXXXXXXXXXXXXXXXX"}

# Conteudo de aula

  ## Aula 1 - Pipeline de Dados

    Reconhecer o que é o Airflow;
    Identificar um processo de Data Pipeline;
    Demonstrar as diferenças entre ETL e ELT
    
  ## Aula 2 - Fontes de Dados

    Elaborar uma requisição para API do Twitter;
    Extrair as informações de json;
    Utilizar a mecânica de resultados por páginas do Twitter.
  
  ## Aula 3 - Lidando com conexão

    Criar e utilizar um ambiente virtual;
    Instalar o Airflow;
    Identificar o que é um Hook;
    Prototipar um Hook;
    Implementar conexões Http no Airflow.

  ## Aula 4 - Tarefa de Extração

    Reconhecer o que é um Operator;
    Elaborar um Operator;
    Identificar o que é um DataLake;
    Relembrar sobre como salvar nossos dados na nossa nova estrutura.

## Aula 5 - Orquestração Airflow