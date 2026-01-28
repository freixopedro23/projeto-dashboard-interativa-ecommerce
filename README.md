# 📊 Dashboard de Análise de E-commerce

Este projeto consiste em uma aplicação web interativa desenvolvida em **Python** utilizando a biblioteca **Dash**. O objetivo é visualizar e analisar estatísticas de vendas de um e-commerce de vestuário, permitindo a exploração de métricas como distribuição de notas, correlação de preços e sazonalidade de vendas.

## 🚀 Funcionalidades e Visualizações

O dashboard apresenta 7 visualizações estratégicas geradas com **Plotly**:

1.  **Histograma de Notas:** Analisa a distribuição de frequência das avaliações dos produtos.
2.  **Scatterplot (Nota vs. Preço):** Explora a correlação entre a nota atribuída ao produto e seu preço.
3.  **Mapa de Calor (Heatmap):** Exibe a matriz de correlação entre variáveis numéricas (Preço, Desconto, Qtd. Vendidos, etc.).
4.  **Barras Horizontais (Sazonalidade):** Mostra o volume de produtos por temporada (ex: Primavera, Verão).
5.  **Gráfico de Pizza (Gênero):** Apresenta a distribuição dos produtos por gênero.
6.  **Gráfico de Densidade:** Visualiza a concentração da quantidade de itens vendidos.
7.  **Regressão Linear:** Relaciona a Nota do produto com a Quantidade de Vendas (com linha de tendência OLS).

## 🛠️ Tecnologias Utilizadas

* **[Python 3.x](https://www.python.org/)**
* **[Dash](https://dash.plotly.com/):** Framework para criação da interface web.
* **[Plotly Express / Figure Factory](https://plotly.com/python/):** Criação dos gráficos interativos.
* **[Pandas](https://pandas.pydata.org/):** Manipulação e análise de dados.
* **[Statsmodels](https://www.statsmodels.org/):** Cálculos estatísticos para a linha de tendência (OLS).

## 📂 Pré-requisitos

Certifique-se de ter o arquivo de dados `ecommerce_estatistica.csv` na raiz do diretório do projeto.

### Instalação das dependências

Utilize o gerenciador de pacotes `pip` para instalar as bibliotecas necessárias:

```bash
pip install dash pandas plotly statsmodels
```

## ▶️ Como Executar
1. Clone este repositório ou baixe os arquivos para sua máquina local.
2. Navegue até o diretório do projeto via terminal.
3. Execute o script Python:
```bash
python app.py
# Ou, se estiver usando Jupyter Notebook, execute todas as células.
```
4. O Dash iniciará um servidor local. Acesse o dashboard no seu navegador através do endereço indicado no terminal, geralmente: http://127.0.0.1:8050/

## 📋 Estrutura do Código
* **ETL e Carregamento:** Leitura do CSV via Pandas (pd.read_csv).
* **Visualização:** Definição dos objetos gráficos (fig1 a fig7).
* **Frontend:** Layout HTML estruturado com dash.html e componentes dcc.Graph.
* **Deploy Local:** Inicialização do servidor em modo de debug (app.run(debug=True)).

---
*Desenvolvido para fins de estudo e análise de dados.*
---
### Próximo passo
Como você está trabalhando com Dash e visualização de dados, gostaria que eu gerasse também um arquivo `requirements.txt` compatível para facilitar a instalação das bibliotecas?
