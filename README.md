# 🚀 Automação de Pipeline e Coleta de Dados de Criptoativos com Python.

Este projeto implementa um pipeline de dados automatizado para coletar, tratar e armazenar indicadores das 15 principais criptomoedas do mercado em tempo real.

---

## 🎯 Objetivo
Automatizar a extração de dados da API do CoinMarketCap para análise de variações de preços e comportamento do mercado em intervalos de alta frequência.

---

## 📂 Estrutura do Projeto

### 1. `Automating Crypto Website API Pull Using Python.ipynb`
O cérebro do projeto. Este Jupyter Notebook executa o pipeline de **ETL** (Extract, Transform, Load):

* **Extração:** Realiza chamadas autenticadas à API enviando requisições e recebendo dados brutos em formato JSON.
* **Transformação:** Utiliza a biblioteca **Pandas** para normalizar estruturas aninhadas e padronizar o dataset.
* **Automação:** Configura um *scheduler* (agendador) interno para repetir a coleta a cada 2 segundos.
* **Carga:** Salva e concatena os novos dados automaticamente em um arquivo físico.

### 2. `API.csv`
O banco de dados gerado pelo script. Ele atua como um histórico consolidado contendo:

* **Ativos:** Nome, símbolo e ranking oficial (CMC).
* **Finanças:** Preços em USD, volume de negociação e Market Cap.
* **Variações:** Histórico de oscilação percentual (1h, 24h, 7d até 90d).
* **Timestamp:** Registro temporal preciso de cada entrada para análise de séries temporais.

 ---

---
*Status do Projeto: 🟢 Operacional*
