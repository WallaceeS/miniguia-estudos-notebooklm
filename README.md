# miniguia-estudos-notebooklm
Repositório dedicado ao projeto da plataforma DIO.

**Contexto**

Escolhi estudar Dados com Python porque tenho interesse em conhecer melhor essa área e entender como Python pode ser usado para trabalhar com dados. Neste caderno, vou estudar desde a organização e limpeza dos dados até sua análise e visualização.

**Objetivos**

Meu objetivo é entender os principais conceitos de análise de dados com Python e conhecer ferramentas e bibliotecas utilizadas nessa área, principalmente o Pandas.

Também quero aprender melhor sobre:

- Manipulação e limpeza de dados;
- DataFrames e Series;
- Análise exploratória de dados;
-  Visualização de dados;
- Uso de Python em situações práticas de análise.

**Curadoria de Fontes**
https://docs.python.org/pt-br/3/tutorial/index.html
https://numpy.org/doc/stable/
[https://pandas.pydata.org/docs/](https://pandas.pydata.org/docs/user_guide/)
https://matplotlib.org/stable/

**Engenharia de Prompts**

**Primeiro Prompt:**

Com base nas fontes disponíveis, quais são as principais etapas envolvidas em um processo de análise de dados utilizando Python? Explique a finalidade de cada etapa e mostre quais ferramentas ou bibliotecas podem ser utilizadas em cada uma delas.

Resultado:

1. Entrada, Leitura e Saída de Dados (I/O)
A análise se inicia com o carregamento e o acesso aos dados brutos para que possam ser manipulados.
No Python básico: É possível realizar a leitura e a escrita de arquivos, bem como salvar dados estruturados utilizando o formato JSON
. A biblioteca padrão do Python também possui recursos para busca de arquivos usando caracteres curinga
.
No NumPy: O pacote fornece rotinas específicas para realizar operações rápidas de entrada e saída (I/O) diretamente em seus objetos de arrays
.
2. Estruturação, Manipulação e Limpeza de Dados
Após o acesso, os dados brutos frequentemente precisam ser organizados, limpos e reestruturados para facilitar as análises.
Estruturas nativas do Python: A linguagem fornece estruturas de dados de alto nível eficientes
, tais como listas, tuplas, conjuntos (sets) e dicionários
, além de ferramentas específicas para trabalhar com listas
.
pandas: Esta biblioteca se destaca por fornecer estruturas de dados de alto desempenho e fáceis de usar, desenhadas especificamente para análise de dados
.
NumPy: Permite a manipulação rápida de conjuntos de dados por meio de rotinas de ordenação (sorting), seleção (selecting) e manipulação de formas (shape manipulation)
.
3. Processamento Matemático e Análise Estatística
Com os dados organizados, realiza-se o processamento numérico para extrair métricas e insights relevantes.
NumPy: Sendo o pacote fundamental para computação científica em Python, ele oferece ferramentas para operações matemáticas e lógicas, álgebra linear básica, operações estatísticas básicas, simulações aleatórias e transformadas discretas de Fourier
.
Python básico: Oferece suporte interno para matemática
 e ferramentas para aritmética decimal com ponto flutuante
.
4. Visualização de Dados
A etapa final consiste em traduzir os dados processados e as descobertas estatísticas em formatos visuais compreensíveis.
Matplotlib: É a biblioteca abrangente voltada para a criação de visualizações estáticas, animadas e interativas, transformando dados complexos em gráficos claro

**Segundo Prompt:**

Quais são as principais funcionalidades do Pandas para manipulação de dados? Organize a resposta por tarefas, como carregamento, seleção, filtragem, transformação e agregação. Para cada tarefa, explique sua finalidade e cite os recursos ou métodos apresentados nas fontes.

Resultado:

. Estruturas de Dados Fundamentais
Antes de manipular os dados, o pandas organiza as informações em duas estruturas principais:
Series: Voltada para dados unidimensionais
.
DataFrame: A estrutura bidimensional principal (em formato de tabela) para gerenciar dados estruturados
.
2. Carregamento de Dados (Importação e Exportação)
O pandas dispõe de um conjunto abrangente de ferramentas de entrada e saída (I/O) para interagir com diversos formatos de arquivos e bancos de dados
:
Arquivos de Texto: Suporte a arquivos de texto plano e CSV
.
Formatos Estruturados e Web: Leitura e escrita em JSON, HTML, XML e tabelas em LaTeX
.
Planilhas: Integração com arquivos do Excel, OpenDocument Spreadsheets (.ods), arquivos binários do Excel (.xlsb) e o motor Calamine
.
Formatos Binários e Big Data: Suporte de alto desempenho para Parquet, Feather, HDF5 (PyTables), Iceberg e ORC
.
Bancos de Dados e Nuvem: Execução de consultas SQL e integração direta com o Google BigQuery
.
Sistemas Estatísticos: Suporte para formatos das ferramentas STATA, SAS e SPSS
.
Outros: Interação com a área de transferência (Clipboard) do sistema operacional e serialização com Pickle
.
3. Seleção de Dados
Para acessar partes específicas de um conjunto de dados, o pandas oferece múltiplos caminhos de indexação e fatiamento
:
Seleção por Rótulo (Label) e Posição: Ferramentas dedicadas para selecionar elementos tanto pelos nomes das linhas/colunas quanto por sua posição numérica
.
Acesso por Atributos: Permite acessar colunas diretamente como atributos do objeto
.
Fatiamento (Slicing): Seleção de intervalos contínuos de linhas ou colunas
.
Seleção por Callable: Uso de funções para definir dinamicamente os critérios de seleção
.
Indexação Hierárquica (MultiIndex): Indexação avançada que permite trabalhar com múltiplas dimensões ou níveis de índices em um único DataFrame
.
Amostragem Aleatória: Seleção de amostras aleatórias (random samples) do conjunto de dados
.
Métodos Rápidos para Escalares: Ferramentas otimizadas para obter e definir valores individuais rapidamente
.
4. Filtragem de Dados
A filtragem permite isolar registros com base em condições lógicas e padrões
:
Indexação Booleana: Filtragem de linhas aplicando máscaras de verdadeiro ou falso
.
Filtragem com isin: Seleção de registros cujos valores pertencem a uma lista predefinida
.
Método where() e Máscaras: Substituição condicional de valores que não atendem a um critério
.
Método query(): Permite realizar consultas e filtragens utilizando expressões em formato de string
.
Detecção de Duplicatas: Identificação e gerenciamento de dados e rótulos duplicados
.
Filtragem de Grupos: Descarte de grupos específicos durante etapas de agrupamento
.
5. Transformação e Reestruturação de Dados
Esta categoria envolve modificar a estrutura física ou os valores contidos nos dados
:
Modelagem de Tabelas (Reshaping): Ferramentas como pivot() e pivot_table() para tabelas dinâmicas, stack() e unstack() para empilhar/desempilhar e melt() ou wide_to_long() para mudar o layout de colunas para linhas
.
Discretização e Codificação: Funções como cut() para categorizar dados contínuos, factorize() para codificar valores e get_dummies() para criar variáveis indicadoras (one-hot encoding)
.
Combinação de Dados (Merge e Join): Operações de união como concat() (concatenação), merge() (junções do tipo banco de dados), join() e junções especializadas como merge_ordered() ou merge_asof() (comum em análises temporais)
.
Dados de Texto: Métodos de string vetorizados (usando o acessor .str) para dividir (split), substituir (replace), concatenar e extrair padrões textuais
.
Tratamento de Dados Ausentes: Identificação, remoção (dropping) e preenchimento (filling) de dados nulos (NA/NaN)
.
Categorias e Tipos de Dados: Suporte para tipos categóricos ordenados e novos tipos nulos (nullable), como inteiros e booleanos que aceitam NA
.
Funções Definidas pelo Usuário (UDFs): Métodos para aplicar funções personalizadas linha a linha ou coluna a coluna
.
6. Agregação e Resumos Estatísticos
Para resumir dados em métricas coletivas ou agrupadas, o pandas conta com
:
Estatísticas Descritivas básicas: Funções rápidas para somar, calcular médias, desvios padrão e outros resumos diretamente nas colunas
.
Group By (Dividir-Aplicar-Combinar): O fluxo clássico de agrupar dados por uma ou mais chaves (splitting), aplicar funções de resumo ou agregação (aggregation) e, por fim, combinar os resultados em uma nova estrutura
.
Operações de Janela (Windowing): Computação de estatísticas móveis através de janelas deslizantes (rolling), expansivas (expanding) ou com pesos exponenciais
.
Funcionalidades de Tempo e Resampling: Suporte especializado para séries temporais que permite alterar a frequência temporal dos dados (resampling) e realizar reduções em intervalos de duração (time deltas)

**Miniguia de Estudo (Entrega Final)**

O que é análise de dados?

A análise de dados é o processo de organizar, tratar, explorar e interpretar dados para encontrar informações relevantes e identificar padrões que possam ajudar na tomada de decisões.

Principais etapas

1. Entrada e leitura dos dados
É o momento de carregar os dados para o ambiente de análise. O Python e bibliotecas como Pandas e NumPy oferecem recursos para trabalhar com diferentes formatos de arquivos.

2. Estruturação e limpeza
Os dados precisam ser organizados e tratados antes da análise. Nessa etapa podem ser identificados valores ausentes, dados duplicados ou informações inconsistentes.

3. Manipulação e análise
Depois de preparados, os dados podem ser filtrados, selecionados, transformados e agrupados para gerar informações e estatísticas.

4. Visualização
Os resultados podem ser apresentados por meio de gráficos, facilitando a identificação de padrões e a interpretação das informações.

Principais bibliotecas

Pandas: manipulação e análise de dados, utilizando estruturas como Series e DataFrame.
NumPy: operações numéricas e computação científica.
Matplotlib: criação de gráficos e visualizações.

** 2. Glossário**

- DataFrame	Estrutura de dados do Pandas organizada em linhas e colunas.
- Series	Estrutura unidimensional utilizada pelo Pandas.
- Dataset	Conjunto de dados utilizado em uma análise.
- EDA	Análise Exploratória de Dados, utilizada para investigar e compreender um conjunto de dados.
- Data Cleaning	Processo de limpeza e tratamento dos dados.
- GroupBy	Recurso utilizado para agrupar dados e realizar operações sobre os grupos.
- NumPy	Biblioteca Python voltada para computação numérica.
- Pandas	Biblioteca utilizada para manipulação e análise de dados.
- Matplotlib	Biblioteca utilizada para criação de visualizações.
- Outlier	Valor que apresenta um comportamento muito diferente dos demais dados.

