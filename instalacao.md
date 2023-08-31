# Instalando python 3.9

## 1 – Atualizando a lista de pacotes e pré-requisitos

  sudo apt update
  sudo apt install software-properties-common

## Instalando o Repositório do Deadsnakes

  sudo add-apt-repository ppa:deadsnakes/ppa

## Instalar a versão 3.9 do Python.

  sudo apt install python3.9

## Instalar o módulo de virtual enviroment da versão 3.9 do python.

  sudo apt install python3.9-venv

## Criar um enviroment. 

  python3.9 -m venv venv

## Ativar o enviroment.  

  source venv/bin/activate

## Instalar a biblioteca requests

  pip install requests==2.27.1

## Fechamando ambiente venv

  deactivate

# Instalando airflow.

## Instalação da versão 2.3.2 do Airflow, 

  AIRFLOW_VERSION=2.3.2

## Salvando-a na variável PYTHON_VERSION

  PYTHON_VERSION=3.9

## Instalar os pacotes de pré-requisitos para o funcionamento do Airflow

  CONSTRAINT_URL="https://raw.githubusercontent.com/apache/airflow/constraints-${AIRFLOW_VERSION}/constraints-${PYTHON_VERSION}.txt"

## Trata-se de um link do GitHub oficial do Airflow e utilizamos os parâmetros de AIRFLOW_VERSION e PYTHON_VERSION para construí-lo.

  pip install "apache-airflow[postgres,celery,redis]==${AIRFLOW_VERSION}" --constraint "${CONSTRAINT_URL}"

## Limpar o nosso terminal.

  clear

## Criando variavel de ambiente do airflow

  export AIRFLOW_HOME=$(pwd)/airflow_pipeline

## Ligando o airflow

  airflow standalone