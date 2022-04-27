# Probabilidade

- [Experimento aleatório](#experimento-aleatório)
  - [Experimento de Bernoulli](#experimento-de-Bernoulli)
- [Espaço amostral](#espaço-amostral)
- [Evento](#evento)
- [Espaço de eventos](#espaço-de-eventos)
- [Função probabilidade](#função-probabilidade)
- [Variável aleatória](#variável-aleatória)
  - [Função massa de probabilidade](#função-massa-de-probabilidade)
  - [Função densidade de probabilidade](#função-densidade-de-probabilidade)
  - [Função distribuição acumulada](#função-distribuição-acumulada)
- [Distribuições de probabilidade](#distribuições-de-probabilidade)
  - [Distribuição binomial](#distribuição-binomial)
  - [Distribuição binomial negativa](#distribuição-binomial-negativa)
  - [Distribuição de Poisson](#distribuição-de-Poisson)
  - [Distribuição normal](#distribuição-normal)
  - [Distribuição qui-quadrado](#distribuição-qui-quadrado)
  - [Distribuição t de Student](#distribuição-t-de-student)
  - [Distribuição F de Snedecor](#distribuição-F-de-Snedecor)

## Experimento aleatório

Experimento aleatório é um processo de observação ou medição com o resultado imprevisível.

### Experimento de Bernoulli

Experimento de Bernoulli é um experimento aleatório com apenas dois resultados possíveis.

Esses dois resultados são convencionalmente denominados sucesso e falha.

## Espaço amostral

Espaço amostral é o conjunto com todos os possíveis resultados de um experimento aleatório.

Esse conjunto é convencionalmente denotado por _Ω_; seus resultados, por _ω_.

## Evento

Evento é um subconjunto com resultados de um espaço amostral.

## Espaço de eventos

Espaço de eventos é conjunto com todos os possíveis eventos.

Esse conjunto é convencionalmente denotado por _𝓕_.

## Função probabilidade

Função probabilidade é uma função que associa um número real para cada evento de um espaço de eventos.

![definição função probabilidade](/imagens/definicao-funcao-probabilidade.png)

Para cada evento _A_, uma função probabilidade deve satisfazer o seguinte axioma:

![primeiro axioma da função probabilidade](/imagens/axioma-funcao-probabilidade-1.png)

Para um espaço amostral _Ω_, uma função probabilidade deve satisfazer o seguinte axioma:

![segundo axioma da função probabilidade](/imagens/axioma-funcao-probabilidade-2.png)

Para um conjunto com eventos mutualmente excludentes _Aᵢ_, uma função probabilidade deve satisfazer o seguinte axioma:

![terceiro axioma da função probabilidade](/imagens/axioma-funcao-probabilidade-3.png)

A probabilidade de um evento pode assumir qualquer número real maior ou igual a 0 e menor ou igual a 1.

## Variável aleatória

Variável aleatória é uma função que associa um número real para cada resultado de um espaço amostral.

![definição variável aleatória](/imagens/definicao-variavel-aleatoria.png)

Variáveis aleatórias podem ser classificadas como:

- discretas caso possam assumir números de um conjunto finito ou infinito enumerável;
- contínuas caso possam assumir números de um conjunto infinito ou não enumerável.

### Função massa de probabilidade

Função massa de probabilidade é uma função que associa probabilidades a resultados de uma variável aleatória discreta.

A função massa de probabilidade de uma variável aleatória discreta _X_ é dada por:

![função massa de probabilidade de uma variável aleatória discreta](/imagens/funcao-massa-probabilidade-variavel-aleatoria-discreta.png)

### Função densidade de probabilidade

Função densidade de probabilidade é uma função que associa probabilidades a resultados infinitesimais de uma variável aleatória contínua.

A função densidade de probabilidade de uma variável aleatória contínua _X_ é dada por:

![função densidade de probabilidade de uma variável aleatória contínua](/imagens/funcao-densidade-probabilidade-variavel-aleatoria-continua.png)

### Função distribuição acumulada

Função distribuição acumulada é uma função que associa probabilidades acumuladas a resultados de uma variável aleatória.

A função distribuição acumulada de uma variável aleatória discreta _X_ é dada por:

![função distribuição acumulada de uma variável aleatória discreta](/imagens/funcao-distribuicao-acumulada-variavel-aleatoria-discreta.png)

A função distribuição acumulada de uma variável aleatória contínua _X_ é dada por:

![função distribuição acumulada de uma variável aleatória contínua](/imagens/funcao-distribuicao-acumulada-variavel-aleatoria-continua.png)

## Distribuições de probabilidade

Distribuições de probabilidade descrevem as probabilidades dos resultados de variáveis aleatórias.

### Distribuição binomial

Uma variável aleatória discreta _X_ com parâmetros _n_ e _p_ e distribuição binomial é denotada por:

![notação de variável aleatória com distribuição binomial](/imagens/notacao-variavel-aleatoria-distribuicao-binomial.png)

A função massa de probabilidade dessa variável é dada por:

![função massa de probabilidade de uma variável aleatória com distribuição binomial](/imagens/funcao-massa-probabilidade-variavel-aleatoria-distribuicao-binomial.png)

A distribuição binomial é associada a uma sequência de experimentos de Bernoulli independentes com:

- _k_ como quantidade de sucessos;
- _n_ como quantidade experimentos realizados;
- _p_ como probabilidade de sucesso em cada experimento.

O gráfico abaixo exibe três distribuições binomiais com dez experimentos e probabilidades de sucesso diferentes.

![gráfico com distribuições binomiais](/imagens/grafico-distribuicoes-binomiais.png)

### Distribuição binomial negativa

Uma variável aleatória discreta _X_ com parâmetros _r_ e _p_ e distribuição binomial negativa é denotada por:

![notação de variável aleatória com distribuição binomial negativa](/imagens/notacao-variavel-aleatoria-distribuicao-binomial-negativa.png)

A função massa de probabilidade dessa variável é dada por:

![função massa de probabilidade de uma variável aleatória com distribuição binomial negativa](/imagens/funcao-massa-probabilidade-variavel-aleatoria-distribuicao-binomial-negativa.png)

A distribuição binomial negativa é associada a uma sequência de experimentos de Bernoulli independentes com:

- _k_ como quantidade de falhas;
- _r_ como quantidade de sucessos;
- _p_ como probabilidade de sucesso em cada experimento.

O gráfico abaixo exibe três distribuições binomiais negativas com dois sucessos e probabilidades de sucesso diferentes.

![gráfico com distribuições binomiais negativas](/imagens/grafico-distribuicoes-binomiais-negativas.png)

### Distribuição de Poisson

Uma variável aleatória discreta _X_ com parâmetro _λ_ e distribuição de Poisson é denotada por:

![notação de variável aleatória com distribuição de Poisson](/imagens/notacao-variavel-aleatoria-distribuicao-poisson.png)

A função massa de probabilidade dessa variável é dada por:

![função massa de probabilidade de uma variável aleatória com distribuição de Poisson](/imagens/funcao-massa-probabilidade-variavel-aleatoria-distribuicao-poisson.png)

A distribuição de Poisson é associada a uma sequência de experimentos de Bernoulli independentes com:

- _k_ como quantidade de sucessos;
- _λ_ como número médio de sucessos em uma determinada exposição.

O gráfico abaixo exibe três distribuições de Poisson com números médios de sucessos diferentes.

![gráfico com distribuições de Poisson](/imagens/grafico-distribuicoes-poisson.png)

### Distribuição normal

Uma variável aleatória contínua _X_ com parâmetros _μ_ e _σ²_ e distribuição normal é denotada por:

![notação de variável aleatória com distribuição normal](/imagens/notacao-variavel-aleatoria-distribuicao-normal.png)

A função densidade de probabilidade dessa variável é dada por:

![função densidade de probabilidade de uma variável aleatória com distribuição normal](/imagens/funcao-densidade-probabilidade-variavel-aleatoria-distribuicao-normal.png)

O gráfico abaixo exibe uma distribuição normal padrão.

![gráfico com distribuição normal padrão](/imagens/grafico-distribuicao-normal-padrao.png)

### Distribuição qui-quadrado

Uma variável aleatória contínua _X_ com parâmetro _v_ e distribuição qui-quadrado é denotada por:

![notação de variável aleatória com distribuição qui-quadrado](/imagens/notacao-variavel-aleatoria-distribuicao-qui-quadrado.png)

O parâmetro _v_ da distribuição qui-quadrado é chamado de graus de liberdade.

A função densidade de probabilidade dessa variável é dada por:

![função densidade de probabilidade de uma variável aleatória com distribuição qui-quadrado](/imagens/funcao-densidade-probabilidade-variavel-aleatoria-distribuicao-qui-quadrado.png)

O gráfico abaixo exibe três distribuições qui-quadrado com graus de liberdade diferentes.

![gráfico com distribuições qui-quadrado](/imagens/grafico-distribuicoes-qui-quadrado.png)

### Distribuição t de Student

Uma variável aleatória contínua _X_ com parâmetro _v_ e distribuição t de Student é denotada por:

![notação de variável aleatória com distribuição t de Student](/imagens/notacao-variavel-aleatoria-distribuicao-t-student.png)

O parâmetro _v_ da distribuição t de Student é denominado graus de liberdade.

A função densidade de probabilidade dessa variável é dada por:

![função densidade de probabilidade de uma variável aleatória com distribuição t de Student](/imagens/funcao-densidade-probabilidade-variavel-aleatoria-distribuicao-t-student.png)

O gráfico abaixo exibe uma distribuição t de Student com cinco graus de liberdade.

![gráfico com distribuição t de Student](/imagens/grafico-distribuicao-t-student.png)

### Distribuição F de Snedecor

Uma variável aleatória contínua _X_ com parâmetros _v1_ e _v2_ e distribuição F de Snedecor é denotada por:

![notação de variável aleatória com distribuição F de Snedecor](/imagens/notacao-variavel-aleatoria-distribuicao-f-snedecor.png)

Os parâmetros _v1_ e _v2_ da distribuição F de Snedecor são denominados graus de liberdade do numerador e do denominador.

A função densidade de probabilidade dessa variável é dada por:

![função densidade de probabilidade de uma variável aleatória com distribuição F de Snedecor](/imagens/funcao-densidade-probabilidade-variavel-aleatoria-distribuicao-f-snedecor.png)

O gráfico abaixo exibe três distribuições F de Snedecor com graus de liberdade diferentes.

![gráfico com distribuições F de Snedecor](/imagens/grafico-distribuicoes-f-snedecor.png)
