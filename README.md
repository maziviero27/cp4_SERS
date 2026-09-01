# CP4 - SERS | Análise de Dados de Energia

Projeto desenvolvido para a disciplina de **Soluções em Energias Renováveis e Sustentáveis (SERS)**, do curso de **Ciência da Computação da FIAP**.

O repositório reúne duas atividades práticas de análise de dados utilizando **Python** e **Pandas**:

1. análise exploratória de seis conjuntos de dados relacionados a consumo e geração de energia;
2. desafio final utilizando dados de carga elétrica obtidos por uma API pública do ONS.

---

## Integrantes

- **Tommaso da C. Nagliatti** — RM 572147
- **Arthur Maziviero Faria** — RM 573928
- **Jun Uehara** — RM 570537
- **Felipe de Souza Gallo** — RM 569680
- **Matheus Martins Lacerda** — RM 570843
- **Roberson Reguero Luiz Junior** — RM 573031

---

## Estrutura do repositório

```text
cp4_SERS/
│
├── CP_04_SERS_ANALISE_COMPLETA.ipynb
├── Desafio_final_todos_desafios_resolvido.ipynb
└── README.md
```

---

# 1. Análise de Datasets de Energia

Arquivo:

```text
CP_04_SERS_ANALISE_COMPLETA.ipynb
```

O primeiro notebook reúne análises de **seis datasets relacionados ao setor energético**.

O objetivo é aplicar operações de manipulação e análise de dados com Pandas, trabalhando com inspeção de DataFrames, filtros, médias, máximos, percentuais, criação de limiares e interpretação dos resultados.

## Dataset 1 - Appliances Energy Prediction

Análise do comportamento energético de uma residência de baixo consumo.

Foram realizadas operações como:

- carregamento e inspeção dos dados;
- renomeação dos atributos;
- identificação do maior consumo dos eletrodomésticos;
- criação de um limiar correspondente a 70% do consumo máximo;
- cálculo da quantidade e do percentual de registros acima do limiar;
- cálculo da temperatura média;
- análise dos registros que apresentam simultaneamente alto consumo e temperatura acima da média;
- comparação e interpretação dos resultados.

---

## Dataset 2 - Steel Industry Energy Consumption

Análise do consumo energético de uma indústria siderúrgica.

O estudo busca identificar situações de consumo elevado e observar se elas coincidem com determinadas condições operacionais.

Foram realizadas análises como:

- inspeção inicial com `head()`, `shape`, `info()` e `describe()`;
- verificação da qualidade dos dados;
- identificação do consumo máximo;
- definição de um limiar de 75% do máximo;
- criação de um DataFrame contendo os registros de alto consumo;
- análise da classificação `Maximum_Load`;
- análise do fator de potência;
- identificação dos registros que combinam alto consumo e fator de potência abaixo de 90%;
- interpretação dos resultados encontrados.

---

## Dataset 3 - Power Consumption of Tetouan City

Análise do consumo de energia em três zonas de distribuição da cidade de Tétouan.

O objetivo é identificar qual zona apresenta o maior pico de consumo e observar as condições registradas nos momentos de maior demanda.

Foram realizados:

- carregamento e organização das três zonas;
- inspeção da amostra;
- cálculo do consumo máximo de cada zona;
- identificação da zona com maior pico;
- criação de um limiar de 70%;
- cálculo da quantidade e percentual de registros acima do limiar;
- comparação dos períodos de alto consumo com a temperatura média;
- interpretação dos DataFrames obtidos.

---

## Dataset 4 - Solar Power Generation Data

Análise de dados de geração de uma planta fotovoltaica.

O objetivo é identificar períodos de alta geração e observar quais inversores aparecem com maior frequência nesses momentos.

Foram realizadas as seguintes etapas:

- carregamento e inspeção dos dados;
- cálculo da potência CA máxima;
- criação de um limiar de 70% da potência máxima;
- filtragem dos períodos de alta geração;
- contagem da frequência dos inversores;
- identificação do inversor mais recorrente;
- interpretação dos resultados.

---

## Dataset 5 - Wind & Solar Energy Production

Análise comparativa de registros de geração de energia solar e eólica.

Como os dois tipos de geração possuem comportamentos e escalas diferentes, os registros foram analisados separadamente.

Foram realizados:

- carregamento e inspeção da amostra;
- separação dos registros solares e eólicos;
- cálculo do valor máximo de cada fonte;
- criação de limiares individuais de 70%;
- criação de DataFrames de alta geração;
- cálculo de quantidades e percentuais;
- comparação entre os resultados de geração solar e eólica.

---

## Dataset 6 - Individual Household Electric Power Consumption

Análise do consumo elétrico de uma residência com monitoramento detalhado.

O objetivo é identificar episódios de demanda elevada que também apresentem corrente acima do comportamento médio.

Foram realizados:

- carregamento e tratamento dos atributos;
- cálculo da potência ativa máxima;
- criação de um limiar de 75%;
- filtragem dos registros de alta demanda;
- cálculo da quantidade e percentual dos registros selecionados;
- cálculo da corrente média;
- criação de um segundo DataFrame com alta potência e corrente acima da média;
- comparação e interpretação dos resultados.

---

# 2. Desafio Final - Análise de Carga Elétrica

Arquivo:

```text
Desafio_final_todos_desafios_resolvido.ipynb
```

O segundo notebook apresenta um desafio completo de análise de dados de carga elétrica utilizando uma **API pública do Operador Nacional do Sistema Elétrico (ONS)**.

A análise utiliza dados da área de carga de **São Paulo (SP)** no período de **01/08/2025 a 07/08/2025**.

O desafio foi dividido em nove etapas.

## Desafio 1 - Construção e inspeção do DataFrame

Os registros retornados pela API foram transformados em um DataFrame Pandas.

Foram realizadas:

- criação do DataFrame;
- exibição dos primeiros registros;
- análise da quantidade de linhas e colunas;
- identificação dos atributos;
- utilização de `info()`;
- utilização de `describe()`;
- identificação das variáveis de área, data/hora e carga elétrica.

---

## Desafio 2 - Organização dos dados

Nesta etapa os dados foram preparados para as análises seguintes.

Foram realizados:

- renomeação dos principais atributos;
- criação de um DataFrame apenas com as colunas necessárias;
- verificação de valores ausentes;
- verificação do tipo da variável de carga;
- tratamento da data e hora;
- registro das decisões de tratamento.

---

## Desafio 3 - Indicadores da carga elétrica

Foram calculados os principais indicadores estatísticos da carga:

- carga mínima;
- carga máxima;
- carga média;
- mediana;
- amplitude entre máximo e mínimo;
- quantidade total de medições.

Esses indicadores foram utilizados para compreender o comportamento geral da carga no período analisado.

---

## Desafio 4 - Períodos de alta demanda

Foi considerado como **alta demanda** todo registro com carga superior a **90% da carga máxima**.

A análise incluiu:

- cálculo do limiar de alta demanda;
- criação de um DataFrame com os registros acima do limiar;
- quantidade de registros;
- percentual em relação ao total;
- maior valor de carga;
- identificação da data e horário do pico.

---

## Desafio 5 - Segundo critério de análise

Além do critério de alta demanda, foi criado um segundo recorte dos dados.

O objetivo foi permitir a comparação entre diferentes condições observadas durante o período analisado.

Foram apresentados:

- critério escolhido pela equipe;
- novo DataFrame;
- quantidade de registros;
- percentual correspondente;
- comparação com o conjunto de alta demanda.

---

## Desafio 6 - Visualização dos dados

Foram desenvolvidos gráficos para facilitar a interpretação dos dados.

Entre as visualizações estão:

- comportamento da carga ao longo do tempo;
- distribuição dos valores de carga.

Cada gráfico é acompanhado de uma interpretação dos resultados observados.

---

## Desafio 7 - Síntese dos resultados

Os principais resultados foram reunidos em uma variável de resumo contendo informações como:

- região;
- período;
- quantidade de registros;
- carga mínima;
- carga máxima;
- carga média;
- mediana;
- limiar de alta demanda;
- quantidade e percentual de alta demanda;
- momento do pico;
- resultado do segundo critério.

---

## Desafio 8 - Relatório técnico

Os indicadores calculados durante a análise foram utilizados para construir um relatório técnico.

O relatório apresenta:

- principais indicadores;
- comportamento da carga;
- pico registrado;
- períodos de alta demanda;
- comparação dos critérios analisados;
- conclusão baseada nos resultados obtidos.

---

## Desafio 9 - Validação crítica

Na etapa final, o relatório foi comparado com os cálculos, DataFrames e gráficos produzidos no notebook.

Foram verificados:

- uso correto dos indicadores;
- afirmações que poderiam ou não ser confirmadas pelos dados;
- possíveis interpretações exageradas;
- possíveis relações de causalidade não demonstradas;
- revisão final do relatório.

A análise final utilizou **336 medições**, com os resultados sendo conferidos diretamente com os cálculos realizados no notebook.

---

# Tecnologias utilizadas

- **Python**
- **Pandas**
- **Jupyter Notebook**
- **Google Colab**
- **Orange Data Mining**
- **API REST**
- **Git**
- **GitHub**

---

# Principais conceitos aplicados

Durante as atividades foram utilizados conceitos como:

- DataFrames;
- leitura e tratamento de dados;
- seleção de colunas;
- renomeação de atributos;
- conversão de tipos;
- tratamento de valores ausentes;
- filtros condicionais;
- estatística descritiva;
- cálculo de médias, medianas, máximos e mínimos;
- limiares percentuais;
- criação de DataFrames derivados;
- cálculo de quantidades e percentuais;
- visualização de dados;
- interpretação de resultados;
- análise crítica de dados.

---

# Como executar

Clone o repositório:

```bash
git clone https://github.com/maziviero27/cp4_SERS.git
```

Entre na pasta do projeto:

```bash
cd cp4_SERS
```

Os notebooks podem ser executados utilizando:

- Google Colab;
- Jupyter Notebook;
- JupyterLab;
- outro ambiente compatível com arquivos `.ipynb`.

Para o primeiro notebook, os arquivos CSV utilizados nas análises devem estar disponíveis no ambiente de execução.

O segundo notebook realiza a consulta dos dados de carga por meio da API utilizada na própria atividade.

---

# Disciplina

**Soluções em Energias Renováveis e Sustentáveis - SERS**

**Checkpoint 04**

FIAP - Faculdade de Informática e Administração Paulista
