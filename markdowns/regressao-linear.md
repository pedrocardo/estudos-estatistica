# Regressão linear

- [Modelo](#modelo)
  - [Equação](#equação)
  - [Notação matricial](#notação-matricial)
- [Variáveis _dummies_](#variáveis-dummies)
  - [_One-hot_ _enconding_](#one-hot-enconding)
- [_Fitted_ _values_](#fitted-values)
- [Resíduos](#resíduos)
- [_Ordinary_ _least_ _squares_](#ordinary-least-squares)
- [Teste F](#teste-f)
- [Teste t de Student](#teste-t-de-student)
- [_R²_](#r)
  - [_R²_ ajustado](#r-ajustado)
- [Normalidade dos resíduos](#normalidade-dos-resíduos)
  - [Teste Shapiro-Wilk](#teste-shapiro-wilk)
- [Resíduos homocedásticos](#resíduos-homocedásticos)
- [Multicolinearidade](#multicolinearidade)
  - [_Variance_ _inflation_ _factor_](#variance-inflation-factor)

## Modelo

Um modelo de regressão linear relaciona uma variável dependente em função de uma ou mais variáveis independentes.

### Equação

A equação de um modelo de regressão linear simples é dada por:

![equação de um modelo de regressão linear simples](/imagens/equacao-modelo-regressao-linear-simples.png)

A equação de um modelo de regressão linear múltipla é dada por:

![equação de um modelo de regressão linear múltipla](/imagens/equacao-modelo-regressao-linear-multipla.png)

Nas equações acima:

- _yᵢ_ representam as variáveis dependentes;
- _xᵢ_ representam as variáveis independentes;
- _p_ representam a quantidade de variáveis independentes;
- _β_ são denominados parâmetros;
- _ε_ são denominados resíduos.

_β₀_ também são denominados _intercepts_ ou coeficientes lineares.

_β₁_ e _βₚ_ também são denominados _slopes_ ou coeficientes angulares.

### Notação matricial

Modelos de regressão linear podem ser representados com notação matricial.

![primeira parte da notação matricial de um modelo de regressão linear](/imagens/notacao-matricial-modelo-regressao-linear-1.png)

![segunda parte da notação matricial de um modelo de regressão linear](/imagens/notacao-matricial-modelo-regressao-linear-2.png)

Nas matrizes acima:

- _n_ representam a quantidade de observações das variáveis;
- _p_ representam a quantidade de variáveis independentes.

A matriz _X_ é denominada _design_ _matrix_.

## Variáveis _dummies_

Variáveis _dummies_ são variáveis quantitativas que podem assumir apenas os valores 0 e 1.

Categorias de variáveis qualitativas podem ser transformadas em variáveis _dummies_.

O valor 0 em uma variável _dummy_ indica a ausência da categoria da variável qualitativa.

O valor 1 em uma variável _dummy_ indica a presença da categoria da variável qualitativa.

|  sabores  | _dummy_ chocolate | _dummy_ baunilha | _dummy_ morango |
| :-------: | :---------------: | :--------------: | :-------------: |
| chocolate |         1         |        0         |        0        |
| baunilha  |         0         |        1         |        0        |
|  morango  |         0         |        0         |        1        |

### _One-hot_ _enconding_

_One-hot_ _enconding_ é um método de criação de variáveis _dummies_ que utiliza uma categoria da variável qualitativa como referência.

O valor 0 em todas as variáveis _dummies_ indica a presença da categoria de referência.

|  sabores  | _dummy_ baunilha | _dummy_ morango |
| :-------: | :--------------: | :-------------: |
| chocolate |        0         |        0        |
| baunilha  |        1         |        0        |
|  morango  |        0         |        1        |

Variáveis _dummies_ transformadas com _one-hot_ _enconding_ podem ser utilizadas em modelos de regressão.

## _Fitted_ _values_

_Fitted_ _values_ são valores estimados por um modelo para a variável dependente.

A equação de um modelo de regressão linear simples com _fitted_ _values_ é dada por:

![equação de modelo de regressão linear simples com fitted values](/imagens/equacao-modelo-regressao-linear-simples-fitted-values.png)

A equação de um modelo de regressão linear múltipla com _fitted_ _values_ é dada por:

![equação de modelo de regressão linear múltipla com fitted values](/imagens/equacao-modelo-regressao-linear-multipla-fitted-values.png)

## Resíduos

Resíduos são as diferenças entre os valores da variável dependente e os _fitted_ _values_ de um modelo.

![fórmula dos resíduos](/imagens/formula-residuos.png)

## _Ordinary_ _least_ _squares_

_Ordinary_ _least_ _squares_ (OLS) é um método para estimar parâmetros de modelos de regressão linear.

Esse método estima parâmetros que minimizem a soma dos quadrados dos resíduos (_residual_ _sum_ _of_ _squares_).

![fórmula da soma dos quadrados dos resíduos](/imagens/formula-soma-quadrados-residuos.png)

A fórmula do vetor com parâmetros de um modelo de regressão linear é dada por:

![fórmula do vetor com parâmetros de um modelo de regressão linear](/imagens/formula-vetor-parametros-modelo-regressao-linear.png)

A fórmula para estimação do parâmetro _β₁_ de um modelo de regressão linear simples é dada por:

![fórmula do parâmetro β₁ de um modelo de regressão linear simples](/imagens/formula-parametro-beta-1-modelo-regressao-linear-simples.png)

A fórmula para estimação do parâmetro _β₀_ de um modelo de regressão linear simples é dada por:

![fórmula do parâmetro β₀ de um modelo de regressão linear simples](/imagens/formula-parametro-beta-0-modelo-regressao-linear-simples.png)

O gráfico abaixo um modelo de regressão linear simples estimado com _ordinary_ _least_ _squares_.

![gráfico com modelo de regressão linear simples estimado com ordinary least squares](/imagens/grafico-modelo-regressao-linear-simples-ordinary-least-squares.png)

## Teste F

Teste F avalia a significância estatística de um modelo de regressão linear.

Esse teste assume, respectivamente, como hipótese nula e hipótese alternativa:

- todos os coeficientes angulares do modelo são estatisticamente iguais a zero;
- pelo menos um coeficiente angular do modelo é estatisticamente diferente de zero.

A fórmula da estatística de teste é dada por:

![fórmula da estatística do teste F](/imagens/formula-estatistica-teste-f-regressao-linear.png)

O p-value da estatística de teste é calculado a partir de uma distribuição F de Snedecor.

![notação de variável aleatória com distribuição F de Snedecor](/imagens/notacao-variavel-aleatoria-distribuicao-f-snedecor.png)

As fórmulas dos graus de liberdade do numerador e do denominador da distribuição F de Snedecor são dadas, respectivamente, por:

![fórmula dos graus de liberdade do numerador da distribuição F de Snedecor](/imagens/formula-graus-liberdade-distribuicao-f-snedecor-numerador.png)

![fórmula dos graus de liberdade do denominador da distribuição F de Snedecor](/imagens/formula-graus-liberdade-distribuicao-f-snedecor-denominador.png)

Nas fórmulas acima:

- _k_ representa a quantidade de parâmetros do modelo.
- _n_ representa a quantidade de observações das variáveis.

## Teste t de Student

Teste t de Student avalia a significância estatística de um determinado parâmetro de um modelo de regressão linear.

Esse teste assume, respectivamente, como hipótese nula e hipótese alternativa:

- o determinado parâmetro do modelo é estatisticamente igual a zero;
- o determinado parâmetro do modelo não é estatisticamente igual a zero.

A fórmula da estatística de teste é dada por:

![fórmula da estatística do teste t de Student](/imagens/formula-estatistica-teste-t-student-regressao-linear.png)

O p-value da estatística de teste é calculado a partir de uma distribuição t de Student.

![notação de variável aleatória com distribuição t de Student](/imagens/notacao-variavel-aleatoria-distribuicao-t-student.png)

A fórmula dos graus de liberdade da distribuição t de Student é dada por:

![fórmula dos graus de liberdade da distribuição t de Student](/imagens/formula-graus-liberdade-distribuicao-t-student.png)

Na fórmula acima:

- _k_ representa a quantidade de parâmetros do modelo.
- _n_ representa a quantidade de observações das variáveis.

## _R²_

_R²_ é uma medida que indica a proporção de variabilidade da variável dependente explicada por um modelo de regressão.

Essa medida também é denominada coeficiente de determinação e sua fórmula é dada por:

![fórmula do R²](/imagens/formula-r-quadrado.png)

### _R²_ ajustado

_R²_ ajustado é uma extensão do _R²_ que compensa a quantidade de variáveis independentes no modelo de regressão.

![fórmula do R² ajustado](/imagens/formula-r-quadrado-ajustado.png)

## Normalidade dos resíduos

Normalidade dos resíduos é assumida pelos testes F e t de Student.

### Teste Shapiro-Wilk

Teste Shapiro-Wilk avalia a normalidade de uma variável aleatória de uma amostra.

Esse teste assume, respectivamente, como hipótese nula e hipótese alternativa:

- a amostra foi selecionada de uma população com distribuição normal.
- a amostra não foi selecionada de uma população com distribuição normal.

A fórmula da estatística de teste é dada por:

![fórmula da estatística de teste Shapiro-Wilk](/imagens/formula-estatistica-teste-shapiro-wilk.png)

Na fórmula acima:

- _x₍ᵢ₎_ são estatísticas de ordem _i_ da amostra;
- _aᵢ_ são constantes geradas a partir de uma amostra de tamanho _n_ e com distribuição normal.

## Resíduos homocedásticos

Resíduos homocedásticos possuem variância constante e independente das observações das variáveis independentes.

O gráfico abaixo exibe resíduos homocedásticos em função dos _fitted_ _values_.

![gráfico com resíduos homocedásticos em função de fitted values](/imagens/grafico-residuos-homocedasticos-fitted-values.png)

Resíduos com variância inconstante são denominados heterocedásticos.

O gráfico abaixo exibe resíduos heterocedásticos em função dos _fitted_ _values_.

![gráfico com resíduos heterocedásticos em função de fitted values](/imagens/grafico-residuos-heterocedasticos-fitted-values.png)

Resíduos heterocedásticos indicam:

- enviesamento dos erros-padrão dos parâmetros, afetando os testes de hipóteses;
- falta de variáveis independentes relevantes no modelo.

## Multicolinearidade

Multicolinearidade é a correlação elevada entre variáveis independentes de um modelo de regressão múltipla.

Essa correlação elevada em modelos de regressão resulta em:

- incapacidade de estimação dos parâmetros;
- parâmetros com variância e erro padrão superestimados;
- parâmetros estatisticamente insignificantes pelos testes t de Student;
- parâmetros com sinais algébricos inesperados;
- _overfitting_.

### _Variance_ _inflation_ _factor_

_Variance_ _inflation_ _factor_ é uma medida que indica quão superestimada é a variância de um parâmetro devido à multicolinearidade.

A fórmula dessa medida é dada por:

![fórmula do variance inflation factor](/imagens/formula-variance-inflation-factor.png)

O _R²ₖ_ é calculado a partir do modelo de regressão linear da variável independente _xₖ_ em função das outras.

![equação do modelo de regressão linear da variável dependente](/imagens/equacao-modelo-regressao-linear-variavel-dependente.png)

Valores de _variance_ _inflation_ _factor_ acima de 5 indicam multicolinearidade.
