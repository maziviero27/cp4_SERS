Checkpoint 01 - Análise de Dados de Energia

Projeto desenvolvido para a disciplina de SERS, com o objetivo de realizar análises exploratórias em diferentes conjuntos de dados relacionados a consumo e geração de energia.

A atividade utiliza Python, Pandas e Orange Data Mining para organizar, tratar, filtrar e interpretar os dados.

Objetivo

O objetivo do projeto é aplicar técnicas de análise de dados para identificar padrões relacionados ao consumo e à geração de energia.

Entre as análises realizadas estão:

cálculo de valores máximos e médias;

criação de limiares de consumo e geração;

filtragem de registros;

cálculo de quantidades e percentuais;

comparação entre diferentes condições;

análise de temperatura, umidade, corrente e fator de potência;

identificação de períodos de alto consumo;

análise de geração solar e eólica;

interpretação dos resultados obtidos.

Tecnologias utilizadas

Python

Pandas

Jupyter Notebook / Google Colab

Orange Data Mining

Git

GitHub

Arquivo principal

O projeto possui um notebook principal contendo as análises realizadas nos diferentes conjuntos de dados:

CP_04_SERS_ANALISE_COMPLETA.ipynb

Análises realizadas

Dataset 1 - Consumo de eletrodomésticos

Análise do consumo energético de eletrodomésticos, buscando identificar períodos de alto consumo e sua relação com variáveis ambientais.

Foram analisados:

consumo máximo;

limiar de 70% do consumo máximo;

quantidade de registros acima do limiar;

temperatura média;

registros de alto consumo com temperatura acima da média.

Dataset 2 - Consumo energético industrial

Análise de dados de consumo de energia em uma indústria siderúrgica.

Foram analisados:

consumo máximo em kWh;

limiar de 75% do consumo máximo;

períodos de alto consumo;

classificação dos tipos de carga;

fator de potência;

situações de alto consumo associadas a fator de potência abaixo de 90%.

Dataset 3 - Consumo de energia por zonas

Análise do consumo de energia em três diferentes zonas de distribuição.

Foram analisados:

consumo máximo de cada zona;

identificação da zona com maior pico;

criação de limiar de 70%;

quantidade e percentual de registros de alto consumo;

temperatura média;

relação entre alto consumo e temperatura acima da média.

Dataset 4 - Geração de energia solar

Análise dos registros de geração de uma planta fotovoltaica.

Foram analisados:

potência máxima;

limiar de 70% da potência máxima;

períodos de alta geração;

frequência dos inversores;

identificação do inversor mais recorrente nos períodos de alta geração.

Dataset 5 - Produção de energia solar e eólica

Análise comparativa dos registros de geração solar e eólica.

Foram analisados:

separação entre dados solares e eólicos;

geração máxima de cada tipo;

limiar individual de 70%;

quantidade de registros de alta geração;

percentual de alta geração;

comparação entre energia solar e eólica.

Dataset 6 - Consumo elétrico residencial

Análise de dados de consumo elétrico residencial.

Foram analisados:

potência ativa máxima;

limiar de 75% da potência máxima;

quantidade e percentual de períodos de alta demanda;

corrente média;

períodos de alta potência associados a corrente acima da média.

Tratamento dos dados

Durante o desenvolvimento foram realizadas etapas de preparação e tratamento dos dados, como:

leitura dos arquivos CSV com Pandas;

tratamento de metadados;

seleção e renomeação de colunas;

conversão de valores para tipos numéricos;

tratamento de valores ausentes;

criação de DataFrames filtrados;

cálculo de métricas e percentuais.

Como executar

Clone o repositório:

git clone LINK_DO_REPOSITORIO

Abra o arquivo:

CP_04_SERS_ANALISE_COMPLETA.ipynb

Execute o notebook no Google Colab, Jupyter Notebook ou em outro ambiente compatível com Python.

Certifique-se de que os arquivos CSV utilizados na atividade estejam disponíveis no ambiente de execução.

Biblioteca utilizada

pip install pandas

Integrantes

Tommaso da C. Nagliatti - RM 572147

Arthur Maziviero Faria - RM 573928

Jun Uehara - RM 570537

Felipe de Souza Gallo - RM 569680

Matheus Martins Lacerda - RM 570843

Roberson Reguero Luiz Junior - RM 573031

Disciplina

SERS - Checkpoint 01: Análise de Dados de Energia

FIAP - Faculdade de Informática e Administração Paulista
