# Projeto de Pipeline ETL para Dados de COVID-19

Este projeto consiste em construir um pipeline ETL (Extract, Transform, Load) para dados de COVID-19 usando arquivos CSV obtidos do [Kaggle COVID-19 Open Datasets for Brazil](https://www.kaggle.com/datasets/cprete/covid19-open-datasets-for-brazil). O pipeline é desenvolvido na Azure, utilizando Databricks e Spark, e organiza os dados em três camadas: Bronze, Silver e Gold.

## Estrutura do Projeto

1. **Download dos Dados**: Os arquivos CSV são baixados do [Kaggle COVID-19 Open Datasets for Brazil](https://www.kaggle.com/datasets/cprete/covid19-open-datasets-for-brazil).
2. **Camada Bronze**: Dados brutos são armazenados na camada Bronze no Azure Data Lake.
3. **Camada Silver**: Dados são limpos e transformados na camada Silver utilizando Databricks e Spark.
4. **Camada Gold**: Dados refinados e agregados são armazenados na camada Gold para análises avançadas e relatórios.

## Tecnologias Utilizadas

- **Azure Data Lake**: Armazenamento de dados brutos e transformados.
- **Azure Databricks**: Plataforma para processamento de dados e criação de pipelines ETL.
- **Apache Spark**: Framework de processamento distribuído para transformar dados.
- **Python**: Linguagem de programação utilizada para scripts e notebooks.

## Como Executar o Projeto

### 1. Configuração do Ambiente

1. **Crie um Workspace no Azure Databricks**:
   - Acesse o [Azure Portal](https://portal.azure.com/) e crie um novo workspace no Azure Databricks.

2. **Configure o Azure Data Lake**:
   - Crie uma conta de armazenamento e um container no Azure Data Lake para armazenar os dados.

3. **Instale o Databricks CLI**:
   - Siga [estas instruções](https://docs.databricks.com/dev-tools/cli/index.html) para instalar e configurar o Databricks CLI.

### 2. Baixe e Prepare os Dados

- Baixe os arquivos CSV do [Kaggle](https://www.kaggle.com/datasets/cprete/covid19-open-datasets-for-brazil).
- Carregue os arquivos no Azure Data Lake na camada Bronze.

### 3. Crie e Execute o Pipeline ETL

1. **Importe os Dados**:
   - Use um notebook Databricks para ler os arquivos CSV e carregá-los na camada Bronze.

2. **Transforme os Dados**:
   - Realize transformações necessárias (limpeza, agregações, etc.) nos dados e armazene o resultado na camada Silver.

3. **Refine e Agregue os Dados**:
   - Faça análises avançadas e agregações dos dados transformados e armazene o resultado na camada Gold.

4. **Analise e Visualize os Dados**:
   - Utilize notebooks Databricks ou conecte-se a ferramentas de BI como Power BI para criar relatórios e dashboards.

### 4. Scripts e Notebooks

- **`notebooks/01_load_data.ipynb`**: Notebook para carregar dados brutos na camada Bronze.
- **`notebooks/02_transform_data.ipynb`**: Notebook para transformar dados e armazenar na camada Silver.
- **`notebooks/03_refine_data.ipynb`**: Notebook para refinar dados e armazenar na camada Gold.

