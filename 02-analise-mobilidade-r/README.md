# Análise Estatística da Mobilidade Urbana com R

## Sobre o projeto

Este projeto apresenta uma análise estatística de uma base de dados sobre mobilidade urbana, desenvolvida no contexto da disciplina **EST 128 – Pacotes Estatísticos II**.

A análise foi realizada utilizando **R**, por meio do **RStudio e Quarto**, combinando procedimentos de estatística descritiva, análise bivariada, inferência estatística e simulação computacional.

O objetivo foi caracterizar os deslocamentos observados e investigar possíveis relações entre características das viagens e o nível de satisfação dos usuários.

## Base de dados

A base utilizada contém **92 observações e 9 variáveis**, relacionadas às características dos deslocamentos realizados pelos usuários. Entre as variáveis estão tipo de viagem, período, meio de transporte, distância percorrida, tempo de deslocamento, custo da viagem, satisfação e chegada pontual.

A base de dados utilizada no projeto também está disponível neste repositório, permitindo consultar os dados utilizados na análise.

## Etapas da análise

O trabalho foi desenvolvido em diferentes etapas:

* Leitura e inspeção dos dados;
* Organização e preparação da base;
* Análise descritiva univariada;
* Análise descritiva bivariada;
* Procedimentos de inferência estatística;
* Simulações computacionais;
* Conclusão.

## Técnicas utilizadas

Entre os procedimentos empregados estão:

* Tabelas de frequência;
* Medidas de tendência central e dispersão;
* Histogramas;
* Gráficos de barras;
* Boxplots;
* Gráficos de dispersão;
* ANOVA;
* Teste de Tukey;
* Teste Qui-Quadrado;
* Regressão linear;
* Simulação de cenários.

## Principais resultados

A análise descritiva indicou predominância de deslocamentos relacionados a trabalho e estudo, além de um nível de satisfação predominantemente moderado entre os usuários. O tempo médio de deslocamento foi de aproximadamente **44,23 minutos**, enquanto o custo médio foi de aproximadamente **R$ 10,66**.
Na análise inferencial, foram identificadas diferenças estatisticamente significativas entre os meios de transporte em relação ao **tempo de deslocamento** e ao **custo da viagem**. Para o tempo, o teste de Tukey indicou diferença significativa entre ônibus e aplicativo. Para o custo, foram identificadas diferenças entre aplicativo e metrô e entre aplicativo e ônibus.

A regressão linear indicou associação estatisticamente significativa entre o **tempo de deslocamento e a satisfação**, com coeficiente angular negativo. O modelo apresentou R² de aproximadamente **31,3%**, indicando que parte da variabilidade da satisfação pode ser explicada pelo tempo de deslocamento na amostra analisada.

Por outro lado, não foram encontradas evidências estatisticamente significativas de associação linear entre **custo da viagem e satisfação**.

Na etapa de simulação, foram avaliados cenários hipotéticos de redução do tempo de deslocamento e do custo da viagem. As simulações indicaram impactos mais expressivos sobre a satisfação prevista quando consideradas reduções no tempo de deslocamento.

## Ferramentas

* R
* RStudio
* Quarto
* ggplot2
* dplyr
* plotly
* fdth
* boot

## Arquivos

* `relatorio-mobilidade-urbana.qmd` — arquivo-fonte contendo o relatório, textos e códigos utilizados na análise.
* `mobilidade-urbana.csv` — base de dados utilizada no projeto.

## Autoria

**Trabalho desenvolvido em grupo no contexto da disciplina EST 128 – Pacotes Estatísticos II.**

## Observação

Este projeto possui caráter acadêmico e foi desenvolvido como atividade da disciplina. As conclusões apresentadas são referentes à amostra analisada e ao contexto do exercício.
