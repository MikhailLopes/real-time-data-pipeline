Project on building a real pipeline

# 📡 Real-Time Data Pipeline with Kafka

## 📌 Descrição
Este projeto consiste na construção de um **pipeline de dados em tempo real** utilizando **Apache Kafka** como sistema de mensageria. O objetivo é processar eventos de logs gerados por aplicações e armazená-los para análise futura.

## 🏗️ Arquitetura Inicial
1. **Produtor (API ou Script)** → Envia logs para o Kafka.
2. **Kafka (Mensageria)** → Encaminha os eventos para os consumidores.
3. **Consumidor (Python/Spark)** → Processa os logs recebidos.
4. **Banco de Dados (PostgreSQL/MongoDB)** → Armazena os logs processados para consulta e análise.

## 🔧 Tecnologias Utilizadas
- **Apache Kafka** – Mensageria para comunicação assíncrona.
- **Python** – Para produtores e consumidores de eventos.
- **Docker** – Para facilitar a implantação do Kafka.
- **PostgreSQL / MongoDB** – Para armazenamento dos dados processados.

## 🚀 Como Executar o Projeto
### 1️⃣ Clonar o repositório:
```sh
 git clone https://github.com/seu-usuario/real-time-data-pipeline.git
 cd real-time-data-pipeline
```
### 2️⃣ Subir o Kafka via Docker:
```sh
 docker-compose up -d
```
### 3️⃣ Executar o produtor de eventos:
```sh
 python producer/producer.py
```
### 4️⃣ Executar o consumidor de eventos:
```sh
 python consumer/consumer.py
```

## 📂 Estrutura do Projeto
```
real-time-data-pipeline/
│── producer/         # Código do produtor de eventos
│── consumer/         # Código do consumidor de eventos
│── database/         # Scripts para banco de dados
│── docs/             # Documentação do projeto
│── docker-compose.yml  # Configuração do Kafka
│── README.md         # Documentação principal
```


