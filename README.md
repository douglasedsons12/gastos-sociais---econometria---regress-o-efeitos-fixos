# Análise Econométrica: Gastos Sociais e Comportamento Eleitoral (2018-2022)

Este repositório apresenta o resumo executivo e os resultados de uma investigação econométrica sobre os determinantes do voto presidencial nos municípios brasileiros, com foco na eficiência dos gastos públicos e indicadores socioeconômicos.

Para visualizar o esboço da pesquisa, o consultar  [Visualizar Resumo Técnico (PDF)](./Parte_Escrita.pdf)

---

##  Objetivo da Pesquisa
Analisar a correlação entre a alocação de recursos municipais (saúde, educação, agricultura) e a performance eleitoral, utilizando o **Índice FIRJAN de Desenvolvimento Municipal (IFDM)** como variável de controle para o nível de desenvolvimento local.

##  Metodologia e Modelagem
Para mitigar o viés de variável omitida e controlar características intrínsecas de cada município que não variam no tempo (como tradições políticas regionais), foi utilizado um **Modelo de Efeitos Fixos (Within-Estimator)** em painel.

### Especificação do Modelo
A equação estimada seguiu a estrutura:

$$pPT_{it} = \beta_{0} + \beta_{1}Gastos_{it} + \beta_{2}IFDM_{it} + \alpha_{i} + \epsilon_{it}$$

Onde:
- **$pPT$**: Proporção de votos no Partido dos Trabalhadores.
- **$\alpha_{i}$**: Efeito fixo municipal (captura heterogeneidade não observada).
- **Teste de Hausman**: Realizado para validar a escolha de Efeitos Fixos sobre Efeitos Aleatórios ($p < 0,05$).

---

##  Insights e Resultados Principais

### 1. O Peso da Saúde e Agricultura
* **Saúde (Atenção Primária):** Verificou-se um impacto positivo e estatisticamente significante. Um incremento de R$ 100 per capita em saúde está associado a um aumento médio de **0,60%** na votação do PT.
* **Agricultura:** Atuou como um forte preditor para o voto oposto (Bolsonarismo). O aumento de gastos nesta função reduziu a proporção de votos no PT em média **1,4%** a cada R$ 100 per capita.

### 2. A Curva do Desenvolvimento (IFDM)
O impacto do desenvolvimento municipal sobre o voto não é linear, mas sim **parabólico**.
* Municípios com **baixo desenvolvimento** (IFDM < 0,517) tendem a apresentar uma relação negativa com o voto à esquerda.
* O retorno eleitoral torna-se positivo apenas após o município ultrapassar esse limiar crítico de desenvolvimento socioeconômico.

### 3. Interação Educação e Renda
A eficácia eleitoral dos gastos em educação mostrou-se dependente do nível de IFDM, sugerindo que o eleitor valoriza o investimento educacional de forma distinta conforme a maturidade econômica do município.

---

##  Documentação Relacionada
Por motivos de propriedade intelectual e confidencialidade de pesquisa, o código-fonte e a base de dados não estão públicos. 
* [Visualizar Resumo Técnico (PDF)](./Parte_Escrita.pdf)

---
**Instituição:** Faculdade de Ciências Econômicas (FACE/UFMG)  
