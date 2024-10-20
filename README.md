# Modelo-de-analise-das-metricas-RFV
Análise de Clusters com Métricas RFM para um E-commerce 🛒

Este projeto visa agrupar clientes de um e-commerce em diferentes clusters com base em suas métricas de compras, utilizando técnicas de clustering. O objetivo é identificar padrões de comportamento e criar estratégias personalizadas de marketing para cada grupo de clientes.

Objetivo
Desenvolver um modelo de clusterização para identificar diferentes perfis de clientes baseados em métricas como frequência de compras, quantidade de itens e valor gasto. O modelo ajudará o e-commerce a personalizar suas campanhas de marketing e aumentar a fidelização de clientes.

Tecnologias Utilizadas
Python (Pandas, Seaborn, Matplotlib, Scikit-learn)
KMeans Clustering
Silhouette Score e Elbow Method
Etapas do Projeto
1. Análise Exploratória de Dados (EDA)
A análise inicial dos dados envolveu a visualização das principais variáveis de interesse, como:

Quantidade de Produtos: Quantos produtos cada cliente compra por transação.
Preço Unitário: O preço dos produtos comprados.
Gráficos de distribuição e boxplots foram usados para detectar outliers e entender melhor a distribuição das variáveis.

2. Pré-processamento dos Dados
Tratamento de Dados Nulos e Duplicados: Remoção de dados inconsistentes.
Normalização: As variáveis numéricas foram normalizadas usando StandardScaler para facilitar a clusterização.
3. Clusterização com KMeans
Utilizamos o algoritmo de KMeans para agrupar os clientes com base em suas compras. Para determinar o número ideal de clusters, aplicamos:

Método do Cotovelo (Elbow Method): Observamos a inércia dos clusters.
Silhouette Score: Avaliamos a coesão dos clusters.
4. Análise dos Clusters
Após a implementação do KMeans, identificamos 5 clusters distintos com base no comportamento dos clientes. Cada cluster foi analisado e interpretado:

Cluster 0: Clientes de alta frequência e alto valor gasto.
Cluster 1: Clientes de baixa frequência e baixo valor.
Cluster 2: Alta frequência, mas valores menores por compra.
5. Visualizações
As visualizações foram essenciais para entender a distribuição dos clientes por cluster e as diferenças em termos de quantidade de produtos e valor gasto.

Gráficos incluídos:

Distribuição de clientes por cluster.
Boxplots de quantidade de produtos e preço unitário por cluster.
6. Sugestões de Ações
Com base nas análises, sugerimos as seguintes ações de marketing:

Clientes de Alta Frequência e Valor Alto: Personalizar campanhas de fidelização com ofertas exclusivas.
Clientes de Baixa Frequência e Valor Baixo: Implementar campanhas de reengajamento.
Clientes de Alta Frequência e Valor Baixo: Oferecer produtos complementares para aumentar o ticket médio.
Conclusão
A clusterização dos clientes permitiu à empresa identificar diferentes perfis de comportamento, o que facilita a criação de campanhas de marketing mais eficazes e personalizadas. Isso ajuda a melhorar a retenção de clientes e aumentar o valor de vida do cliente (LTV).

Como Executar o Projeto
Clone o repositório:
bash
Copiar código
git clone https://github.com/seu-usuario/seu-repositorio.git
Instale as dependências:
bash
Copiar código
pip install -r requirements.txt
Execute o Jupyter Notebook ou o script Python com os dados:
bash
Copiar código
python clustering_rfm.py
Arquivos do Projeto
clustering_rfm.py: Código principal com a implementação do modelo.
data.csv: Base de dados de transações de e-commerce.
visualizações: Pasta com gráficos gerados durante a análise.
 
