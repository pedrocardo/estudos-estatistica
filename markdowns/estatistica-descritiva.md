# Estatística descritiva

- [Tabela de distribuição de frequências](#Tabela-de-distribuição-de-frequências)
- [Tabela de contingência](#Tabela-de-contingência)
- [Medidas-resumo](#Medidas-resumo)
  - [Medidas-resumo de tendência central](#Medidas-resumo-de-tendência-central)
    - [Média aritmética simples](#Média-aritmética-simples)
    - [Média aritmética ponderada](#Média-aritmética-ponderada)
    - [Mediana](#Mediana)
  - [Medidas-resumo separatrizes](#Medidas-resumo-separatrizes)
    - [Percentis](#Percentis)
    - [Decis](#Decis)
    - [Quartis](#Quartis)
  - [Medidas-resumo de dispersão](#Medidas-resumo-de-dispersão)
    - [Amplitude](#Amplitude)
    - [Amplitude interquartil](#Amplitude-interquartil)
    - [Variância](#Variância)
    - [Desvio padrão](#Desvio-padrão)
    - [Erro padrão](#Erro-padrão)
- [Medidas de correlação](#Medidas-de-correlação)
  - [Covariância](#Covariância)
  - [Coeficiente de correlação de Pearson](#Coeficiente-de-correlação-de-Pearson)
- [Gráficos](#Gráficos)
  - [Gráfico de barras](#Gráfico-de-barras)
  - [_Boxplot_](#Boxplot)
  - [Histograma](#Histograma)
  - [Gráfico de dispersão](#Gráfico-de-dispersão)
- [Padronização por _z-scores_](#Padronização-por-z-scores)

## Tabela de distribuição de frequências

Tabela de distribuição de frequências é uma matriz bidimensional com as quantidades de ocorrências dos dados de uma variável agrupados.

Essa tabela pode apresentar frequências absolutas, acumuladas, relativas e relativas acumuladas.

Dados de variáveis qualitativas podem ser agrupados conforme as próprias categorias possíveis da variável.

|  espécie  | frequência absoluta | frequência acumulada | frequência relativa | frequência relativa acumulada |
| :-------: | :-----------------: | :------------------: | :-----------------: | :---------------------------: |
|  Adelie   |         146         |         146          |      0.4384384      |           0.4384384           |
| Chinstrap |         68          |         214          |      0.2042042      |           0.6426426           |
|  Gentoo   |         119         |         333          |      0.3573574      |               1               |

Dados de variáveis quantitativas podem ser agrupados em intervalos numéricos.

|   massa   | frequência absoluta | frequência acumulada | frequência relativa | frequência relativa acumulada |
| :-------: | :-----------------: | :------------------: | :-----------------: | :---------------------------: |
| 2700-3900 |         150         |         150          |      0.4504505      |           0.4504505           |
| 3901-5100 |         128         |         278          |      0.3843844      |           0.8348349           |
| 5101-6300 |         55          |         333          |      0.1651652      |               1               |

## Tabela de contingência

Tabela de contingência é uma matriz bidimensional com as frequências conjuntas dos dados de duas variáveis agrupados.

Essa tabela pode apresentar frequências absolutas ou relativas e totais marginais.

Dados de variáveis qualitativas podem ser agrupados conforme as próprias categorias possíveis da variável.

|           | Biscoe | Dream | Torgersen | Total |
| :-------- | :----: | :---: | :-------: | :---: |
| Adelie    |   44   |  56   |    52     |  152  |
| Chinstrap |   0    |  68   |     0     |  68   |
| Gentoo    |  124   |   0   |     0     |  124  |
| Total     |  168   |  124  |    52     |  344  |

## Medidas-resumo

Medidas-resumo são valores que representam informações sobre a distribuição dos dados de uma variável.

As medidas-resumo descritas abaixo só podem ser calculadas para variáveis quantitativas.

### Medidas-resumo de tendência central

#### Média aritmética simples

Média aritmética simples é a soma dos dados dividida pela quantidade de elementos.

![fórmula da média aritmética simples populacional](/imagens/formula-media-aritmetica-simples-populacional.png)

![fórmula da média aritmética simples amostral](/imagens/formula-media-aritmetica-simples-amostral.png)

#### Média aritmética ponderada

Média aritmética ponderada é a soma dos dados multiplicados por pesos, dividida pela soma dos pesos.

![fórmula da média aritmética ponderada populacional](/imagens/formula-media-aritmetica-ponderada-populacional.png)

![fórmula da média aritmética ponderada amostral](/imagens/formula-media-aritmetica-ponderada-amostral.png)

#### Mediana

Mediana é o valor que corresponde ao dado na posição central dos dados ordenados.

Caso a quantidade de elementos seja par, a mediana corresponde ao valor da média dos dois dados nas posições centrais.

### Medidas-resumo separatrizes

As medidas separatrizes descritas abaixo são denominadas quantis.

#### Percentis

Percentis são valores que dividem os dados em cem partes com dimensões iguais.

Por exemplo, o primeiro percentil é um valor maior ou igual a 1% e menor ou igual a 99% dos dados.

#### Decis

Decis são valores que dividem os dados em dez partes com dimensões iguais.

Por exemplo, o primeiro decil é um valor maior ou igual a 10% e menor ou igual a 90% dos dados.

#### Quartis

Quartis são valores que dividem os dados em quatro partes com dimensões iguais.

Por exemplo, o primeiro quartil é um valor maior ou igual a 25% e menor ou igual a 75% dos dados.

### Medidas-resumo de dispersão

#### Amplitude

Amplitude é a diferença entre o maior e o menor dado.

![fórmula da amplitude](/imagens/formula-amplitude.png)

#### Amplitude interquartil

Amplitude interquartil é a diferença entre o 3° e o 1° quartil.

![fórmula da amplitude interquartil](/imagens/formula-amplitude-interquartil.png)

#### Variância

Desvios são as diferenças entre os dados e a média.

Variância populacional é a soma dos quadrados dos desvios, dividida pela quantidade de elementos.

![fórmula da variância populacional](/imagens/formula-variancia-populacional.png)

Variância amostral é a soma dos quadrados dos desvios, dividida pela quantidade de elementos menos um.

![fórmula da variância amostral](/imagens/formula-variancia-amostral.png)

#### Desvio padrão

Desvio padrão é a raiz quadrada da variância.

![fórmula do desvio padrão populacional](/imagens/formula-desvio-padrao-populacional.png)

![fórmula do desvio padrão amostral](/imagens/formula-desvio-padrao-amostral.png)

#### Erro-padrão

Amostras da mesma população e com o mesmo tamanho podem ter valores diferentes para a mesma estatística.

Erro-padrão é o desvio padrão de uma estatística.

Erro-padrão da média amostral é o desvio padrão dividido pela raiz quadrada da quantidade de elementos.

![fórmula do erro-padrão da média amostral](/imagens/formula-erro-padrao-media-amostral.png)

## Medidas de correlação

Medidas de correlação são valores que representam a relação entre os dados de duas variáveis quantitativas.

### Covariância

Desvios são as diferenças entre os dados e a média.

Covariância populacional é a soma dos produtos dos desvios, dividida pela quantidade de elementos.

![fórmula da covariância populacional](/imagens/formula-covariancia-populacional.png)

Covariância amostral é a soma dos produtos dos desvios, dividida pela quantidade de elementos menos um.

![fórmula da covariância amostral](/imagens/formula-covariancia-amostral.png)

### Coeficiente de correlação de Pearson

Coeficiente de correlação de Pearson é a covariância dividida pelo produto dos desvios padrão.

![fórmula do coeficiente de correlação de Pearson populacional](/imagens/formula-coefieciente-correlacao-pearson-populacional.png)

![fórmula do coeficiente de correlação de Pearson amostral](/imagens/formula-coefieciente-correlacao-pearson-amostral.png)

Essa medida pode assumir qualquer número real maior ou igual a -1 e menor ou igual a 1.

Variáveis com correlação igual a zero não possuem relação linear.

## Gráficos

### Gráfico de barras

Gráfico de barras é um gráfico para representação da distribuição de frequências dos dados de uma variável qualitativa.

![gráfico de barras](/imagens/grafico-barras.png)

As barras representam as categorias possíveis da variável.

Os tamanhos das barras são proporcionais às frequências dos dados em cada categoria.

### _Boxplot_

_Boxplot_ é um gráfico para representação da distribuição dos dados de uma variável quantitativa.

![boxplot](/imagens/grafico-boxplot.png)

As linhas horizontais, que formam o retângulo, representam o 1°, 2° e 3° quartil.

As linhas horizontais nas pontas da linha vertical representam o valor mínimo e máximo dos dados desconsiderando _outliers_.

Os círculos representam _outliers_.

### Histograma

Histograma é um gráfico para representação da distribuição de frequências dos dados de uma variável quantitativa.

![histograma](/imagens/grafico-histograma.png)

As barras representam os intervalos numéricos em que os dados estão agrupados.

Os tamanhos das barras são proporcionais às frequências dos dados em cada intervalo numérico.

### Gráfico de dispersão

Gráfico de dispersão é um gráfico para representação dos dados de duas variáveis quantitativas como coordenadas cartesianas.

![gráfico de dispersão](/imagens/grafico-dispersao.png)

## Padronização por _z-scores_

Padronização é o processo de adequação dos dados de uma variável para um determinado padrão.

Escores padrão ou _z-scores_ são os desvios (diferenças entre os dados e a média) divididos pelo desvio padrão de uma variável.

![fórmula do z-score populacional](/imagens/formula-zscore-populacional.png)

![fórmula do z-score amostral](/imagens/formula-zscore-amostral.png)

Variáveis padronizadas por _z-scores_ possuem média igual a 0 e desvio padrão igual a 1.
