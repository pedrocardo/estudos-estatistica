# Estatística inferencial

- [Amostragem](#amostragem)
- [Teste de hipóteses](#teste-de-hipóteses)
  - [Hipótese nula](#hipótese-nula)
  - [Hipótese alternativa](#hipótese-alternativa)
  - [Estatística de teste](#estatística-de-teste)
  - [_p-value_](#p-value)
  - [Tipos de erros](#tipos-de-erros)
  - [Nível de significância](#nível-de-significância)
  - [Região crítica](#região-crítica)
  - [Testes unilaterais](#testes-unilaterais)
  - [Testes bilaterais](#testes-bilaterais)
  - [Decisão](#decisão)
- [Teste t de Student](#teste-t-de-Student)
  - [Para uma amostra](#para-uma-amostra)
  - [Para duas amostras independentes](#para-duas-amostras-independentes)
- [Teste t de Welch](#teste-t-de-Welch)

## Amostragem

Amostragem é o processo de selecionar elementos de uma população para comporem uma amostra.

## Teste de hipóteses

Teste de hipóteses são procedimentos para avaliação de hipóteses sobre parâmetros de populações.

Esses testes são utilizados para inferir conclusões sobre populações a partir de amostras.

### Hipótese nula

Hipótese nula é um pressuposto sobre parâmetros de uma ou mais populações.

Essa hipótese é convencionalmente denotada por _H₀_.

### Hipótese alternativa

Hipótese alternativa é um pressuposto considerado como verdadeiro caso a hipótese nula seja rejeitada.

Essa hipótese é convencionalmente denotada por _H₁_.

### Estatística de teste

Estatística de teste é uma medida utilizada para testar a hipótese nula.

### _p-value_

_p-value_ é a probabilidade de obter-se um valor igual ou mais extremo que o calculado para a estatística de teste.

Essa probabilidade é calculada a partir da distribuição da estatística de teste.

### Tipos de erros

A avaliação das hipóteses nula e alternativa pode resultar em dois tipos de erros.

| decisão                      | hipótese nula verdadeira | hipótese nula falsa |
| :--------------------------- | :----------------------: | :-----------------: |
| rejeitar a hipótese nula     |      erro do tipo 1      |     nenhum erro     |
| não rejeitar a hipótese nula |       nenhum erro        |   erro do tipo 2    |

### Nível de significância

Nível de significância é a probabilidade pré-estabelecida de cometer o erro do tipo 1.

Essa probabilidade é convencionalmente denotada por _α_.

### Região crítica

Região crítica são os valores da estatística de teste com _p-value_ menor ou igual ao nível de significância pré-estabelecido.

### Testes unilaterais

Testes unilaterais são testes com a região crítica em uma das caudas da distribuição de probabilidade da estatística de teste.

O gráfico abaixo exibe uma distribuição t de Student com cinco graus de liberdade e região crítica a esquerda com _α_ = 5%.

![gráfico com distribuição t de Student com região crítica a esquerda](/imagens/grafico-distribuicao-t-student-regiao-critica-unilateral-esquerda.png)

O gráfico abaixo exibe uma distribuição qui-quadrado com quatro graus de liberdade e região crítica a direita com _α_ = 5%.

![gráfico com distribuição qui-quadrado com região crítica a direita](/imagens/grafico-distribuicao-qui-quadradado-regiao-critica-unilateral-direita.png)

### Testes bilaterais

Testes bilaterais são testes com a região crítica dividida nas duas caudas da distribuição de probabilidade da estatística de teste.

O gráfico abaixo exibe uma distribuição t de Student com cinco graus de liberdade e região crítica bilateral com _α_ = 5%.

![gráfico com distribuição t de Student com região crítica bilateral](/imagens/grafico-distribuicao-t-student-regiao-critica-bilateral.png)

### Decisão

A hipótese nula deve ser aceita se o _p-value_ for maior que o nível de significância pré-estabelecido para o teste.

A hipótese nula deve ser rejeitada se o _p-value_ for menor que o nível de significância pré-estabelecido para o teste.

## Teste t de Student

Teste t de Student avalia diferenças entre médias populacionais.

### Para uma amostra

Para uma amostra, o teste t de Student assume como hipótese nula: _μ_ - _μ₀_ = 0.

A fórmula da estatística de teste é dada por:

![fórmula da estatística de teste t de Student para uma amostra](/imagens/formula-estatistica-teste-t-student-uma-amostra.png)

O _p-value_ da estatística de teste é calculado a partir de uma distribuição t de Student com:

![fórmula dos graus de liberdade do teste t de Student para uma amostra](/imagens/formula-graus-liberdade-teste-t-student-uma-amostra.png)

O teste t de Student pode assumir as seguintes hipóteses alternativas:

- _μ_ - _μ₀_ < 0 para um teste unilateral à esquerda;
- _μ_ - _μ₀_ > 0 para um teste unilateral à direita;
- _μ_ - _μ₀_ ≠ 0 para um teste bilateral.

### Para duas amostras independentes

Para duas amostras independentes de populações com variâncias homogêneas, o teste t de Student assume como hipótese nula: _μ₁_ - _μ₂_ = 0.

A fórmula da estatística de teste é dada por:

![primeira parte da fórmula estatística de teste t de Student para duas amostras independentes](/imagens/formula-estatistica-teste-t-student-duas-amostras-independentes-1.png)

![segunda parte da fórmula estatística de teste t de Student para duas amostras independentes](/imagens/formula-estatistica-teste-t-student-duas-amostras-independentes-2.png)

O _p-value_ da estatística de teste é calculado a partir de uma distribuição t de Student com:

![fórmula dos graus de liberdade do teste t de Student para duas amostras independentes](/imagens/formula-graus-liberdade-teste-t-student-duas-amostras-independentes.png)

O teste t de Student pode assumir as seguintes hipóteses alternativas:

- _μ₁_ - _μ₂_ < 0 para um teste unilateral à esquerda;
- _μ₁_ - _μ₂_ > 0 para um teste unilateral à direita;
- _μ₁_ - _μ₂_ ≠ 0 para um teste bilateral.

## Teste t de Welch

Teste t de Welch avalia a diferença entre as médias de duas populações com variâncias não homogêneas.

Esse teste assume como hipótese nula: _μ₁_ - _μ₂_ = 0.

A fórmula da estatística de teste é dada por:

![fórmula da estatística de teste t de Welch](/imagens/formula-estatistica-teste-t-welch.png)

O _p-value_ da estatística de teste é calculado a partir de uma distribuição t de Student com:

![fórmula dos graus de liberdade do teste t de Welch](/imagens/formula-graus-liberdade-teste-t-de-welch.png)

O teste t de Welch pode assumir as seguintes hipóteses alternativas:

- _μ₁_ - _μ₂_ < 0 para um teste unilateral à esquerda;
- _μ₁_ - _μ₂_ > 0 para um teste unilateral à direita;
- _μ₁_ - _μ₂_ ≠ 0 para um teste bilateral.
