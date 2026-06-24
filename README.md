# DataView — Exploração e Análise de Dados de Vendas

## Sobre o projeto
O DataView é um projeto de análise exploratória de dados (EDA) de vendas,
desenvolvido em Python no Google Colab. O notebook lê, limpa, transforma,
analisa e visualiza um dataset sintético de vendas de produtos de tecnologia,
gerando métricas, insights e relatórios exportáveis.

## O que o projeto analisa
- Receita total e volume de vendas por mês, trimestre e dia da semana
- Top 5 produtos e categorias por receita
- Desempenho por região com ticket médio
- Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro)
- Produto favorito de cada cliente
- Comparação entre dados com e sem tratamento de outliers (v1 e v2)
- Exportação de relatórios em CSV e JSON

## Objetivo
Praticar os principais conceitos de Python e análise de dados:
- Lógica de programação com Python
- Variáveis, tipos de dados e operadores
- Condicionais (if, elif, else) e repetição (for, while)
- Funções com parâmetros, retorno e funções lambda
- Funções de ordem superior (callback)
- Leitura e escrita de arquivos CSV e JSON
- Módulo datetime para manipulação de datas
- Expressões regulares com o módulo re
- Pandas: DataFrames, limpeza, groupby, filtros e transformações
- NumPy: arrays, operações vetorizadas, broadcasting e boolean indexing
- Detecção e tratamento de outliers com método IQR
- Matplotlib e Seaborn: gráficos, customização e exportação em PNG
- Versionamento com GitHub

## Decisão de versão
Foi escolhida a versão **v2 (outliers removidos)** como base da análise final.
A versão v1 está disponível em `data/processed/v1_com_outliers/` para consulta.

## Como executar
### No Google Colab (recomendado)
1. Acesse [Google Colab](https://colab.research.google.com)
2. Faça upload do arquivo `notebooks/dataview.ipynb`
3. Execute as células na ordem, de cima para baixo

### Localmente com VS Code
1. Instale o Python 3.10+ e o VS Code
2. Instale as dependências:
pip install pandas numpy matplotlib seaborn
3. Abra o arquivo `notebooks/dataview.ipynb` e execute as células

## Estrutura do projeto
dataview/

├── data/

│   ├── raw/                        # Dataset bruto gerado

│   ├── processed/

│   │   ├── v1_com_outliers/        # Dados limpos, outliers mantidos

│   │   └── v2_outliers_tratado/    # Dados limpos, outliers removidos

│   └── final/                      # Dataset final para uso futuro

├── notebooks/

│   └── dataview.ipynb              # Notebook principal

├── outputs/

│   ├── metricas_por_mes.csv        # Métricas mensais

│   ├── segmentacao_clientes.csv    # Segmentação de clientes

│   ├── estatisticas_gerais.json    # Estatísticas gerais

│   └── graficos/                   # Gráficos exportados em PNG

└── README.md

## Resultados do pipeline
| Etapa | Registros |
|---|---|
| Dataset bruto gerado | 180 |
| Após limpeza — v1 | 162 |
| Após outliers — v2 | 150 |
| Dataset final analisado | 150 |
| Receita total analisada | R$ 777.552,00 |
| Clientes segmentados | 30 |

## Ferramentas utilizadas
- Python 3.10+
- Google Colab
- Pandas, NumPy, Matplotlib, Seaborn
- Módulos: re, datetime, os, json, random
- GitHub para versionamento

## Vídeo de demonstração
- https://www.loom.com/share/e2a79bb1c2cc428ab8bb43ec829c4e14
