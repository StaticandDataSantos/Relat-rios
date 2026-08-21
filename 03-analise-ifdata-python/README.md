# Análise Exploratória de Instituições Financeiras com Python

## Sobre o projeto

Este projeto apresenta uma análise exploratória dos dados de instituições financeiras disponibilizados pela plataforma IFData, do Banco Central do Brasil.

A análise foi desenvolvida em Python utilizando um Jupyter Notebook, com foco no carregamento, tratamento, exploração e visualização dos dados.

O projeto busca demonstrar a aplicação de ferramentas de análise de dados para compreender características financeiras e estruturais das instituições presentes na base.

## Base de dados

A base utilizada corresponde aos dados do IFData referentes a setembro de 2025, disponibilizados pelo Banco Central do Brasil.

A base original possui 1.499 registros e 19 colunas, contendo informações sobre instituições financeiras, localização, classificação regulatória e indicadores financeiros.

Entre as principais variáveis estão:

- Instituição;
- Código;
- TCB;
- Segmento (SR);
- Tipo de controle (TC);
- Cidade;
- UF;
- Ativo Total;
- Carteira de Crédito;
- Títulos e Valores Mobiliários;
- Passivo Exigível;
- Captações;
- Patrimônio Líquido;
- Lucro Líquido;
- Número de Agências;
- Número de Postos de Atendimento.

## Etapas da análise

O projeto foi desenvolvido em etapas:

1. Importação das bibliotecas e configuração do ambiente;
2. Carregamento e inspeção inicial dos dados;
3. Limpeza e preparação da base;
4. Criação de variáveis derivadas;
5. Verificação da qualidade dos dados;
6. Análise exploratória;
7. Estatísticas descritivas;
8. Análise por segmentos;
9. Visualização dos dados;
10. Análise de correlação;
11. Interpretação dos resultados.

## Tratamento dos dados

Durante o processo de preparação foram removidos registros que não representavam instituições individuais e observações sem informações necessárias para a análise.

As variáveis financeiras, originalmente armazenadas como texto, foram convertidas para valores numéricos.

Também foram removidas duplicidades e criado um novo índice para a base tratada.

Além disso, foram criadas variáveis derivadas para ampliar a análise, incluindo:

- ROE (Retorno sobre o Patrimônio);
- Índice entre Carteira de Crédito e Ativo Total;
- Classificação entre instituições digitais e tradicionais;
- Tipo de controle da instituição.

## Análises realizadas

Entre as análises desenvolvidas estão:

- Estatísticas descritivas;
- Distribuição das instituições por segmento;
- Distribuição por tipo de controle;
- Comparação entre instituições digitais e tradicionais;
- Análise agregada por segmento;
- Ranking das instituições por Ativo Total;
- Participação dos ativos segundo o tipo de controle;
- Distribuição do ROE por segmento;
- Matriz de correlação entre variáveis financeiras e estruturais.

As visualizações foram produzidas utilizando principalmente Matplotlib e Seaborn.

## Principais resultados

Após o processo de limpeza, a base utilizada nas análises passou a conter 1.419 registros.

A comparação entre média e mediana do Ativo Total revelou uma diferença expressiva. A média foi de aproximadamente R$ 12,65 milhões, enquanto a mediana foi de aproximadamente R$ 257,66 mil.

Essa diferença indica uma distribuição assimétrica, influenciada pela presença de instituições com volumes de ativos muito elevados. Dessa forma, a mediana apresenta uma representação mais adequada da instituição típica da base.

Também foram identificadas 66 instituições com ROE superior a 15%, segundo o critério adotado na análise.

A correlação entre o Número de Agências e o Ativo Total foi de aproximadamente 0,07, indicando uma associação linear muito fraca entre essas variáveis.

## Ferramentas utilizadas

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Arquivos

- `analise-ifdata-python.ipynb` — notebook contendo o código, as análises, visualizações e interpretações.
- `IFData-09-2025.csv` — base de dados utilizada no projeto.

## Fonte dos dados

Banco Central do Brasil — IFData.

https://www3.bcb.gov.br/ifdata

## Observação

Este projeto possui finalidade acadêmica e foi desenvolvido como exercício de análise de dados.

Os resultados apresentados referem-se à base disponibilizada para setembro de 2025 e não representam, isoladamente, uma avaliação atual do sistema financeiro brasileiro.

