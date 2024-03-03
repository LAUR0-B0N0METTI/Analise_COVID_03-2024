# Análise dos Casos de COVID-19 no Brasil (2024)

## Introdução

Neste estudo estão sendo explorados os dados dos casos de COVID-19 no Brasil ao longo de 2024 até o mês de março, utilizando o conjunto de dados proveniente do arquivo CSV "HIST_PAINEL_COVIDBR_2024_Parte1_27fev2024" disposto para download no site do Ministério da Saúde. O  objetivo é fornecer uma análise aprofundada, revelando insights valiosos sobre a evolução da pandemia em diferentes níveis geográficos e temporais.

## Carregamento e Exploração dos Dados

Os dados foram carregados e manipulados com a biblioteca pandas do Python, revelando um conjunto de 309.045 registros distribuídos em 17 colunas. Essas colunas abrangem uma variedade de informações, desde a região geográfica até métricas específicas de saúde, como casos acumulados, óbitos e dados demográficos. A seguir, destacamos algumas análises preliminares:

### Resumo Geral dos Dados

```python
dados_covid.info()
```

A análise preliminar mostra a diversidade das variáveis presentes no conjunto de dados, permitindo-nos explorar a fundo as nuances dos impactos da pandemia.

## Análise Exploratória dos Dados 

### Visualização Gráfica

   A análise gráfica revela tendências nos novos casos da variante, fornecendo insights sobre a disseminação e impacto dessa variante específica.

1. **Novos Casos da Variante:** <br>
![alt text](<Novos casos da variante-1.png>)

2. **Casos Acumulados da Variante:** <br>
![alt text](<Casos acumulados da variante-1.png>)
 
3. **Novos obitos** <br>
![alt text](<Novos obitos-1.png>)

4. **Obitos acumulados** <br>
![alt text](<Obitos acumulados-1.png>)


## Estatísticas Descritivas

### Visão Detalhada

```python
dados_covid.describe(include='all')
```

A análise estatística oferece uma visão abrangente das métricas presentes no conjunto de dados, incluindo médias, desvios padrão e percentis.

## Correlações entre Variáveis

### Exploração das Relações

```python
dados_covid.corr()
```

A matriz de correlação destaca relações entre variáveis, indicando padrões que podem influenciar os resultados observados.

## Identificação de Outliers

### Investigação de Registros Atípicos

```python
dados_covid.sort_values(by=['obitosNovos']).head()
```

A identificação de outliers fornece insights valiosos sobre eventos excepcionais que merecem atenção especial.

## Conclusão

Este resumo destaca apenas uma fração das análises realizadas. O arquivo Analise_Covid.ipynb correspondente contém o código-fonte completo e visualizações interativas para uma exploração mais detalhada.

A compreensão detalhada desses dados não apenas contribui para nossa visão sobre a pandemia atual, mas também orienta estratégias futuras para a gestão da saúde pública.

<br>
<br>

**Autor**<br>
[ Lauro Bonometti ]
