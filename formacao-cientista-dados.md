# Formação Cientista de Dados - Udemy

Esté um arquivo de resumo com todos os conteúdos e links que serviram de estudo no curso de Formação em Cientista de Dados da Udemy([Link](https://www.udemy.com/cientista-de-dados/))

## Roadmap do curso

## Estatística

### Conceitos:

#### Amostra

É um conjunto da população que se propõe analisar.

Características:
* Reflete a população com suas características;
* É usada em detrimento da população pela relação custo / benefício. Tem-se como exemplo, a pesquisa de intenção de voto realizada em época de eleição.

Tipos:
* Aleatória simples: e quando de um todo da população, se extrai a amostra, de maneira que todos tenham iguais chances de entrar.
  * Com reposição: é quando um item foi retirado da amostra, mas pode retornar, podendo novamente ser capturado para amostra. Exemplo: testes antidoping
  * Sem reposição: é quando um item, após ser retirado da população para a amostra, não pode ser recolocado. Exemplo: pesquisa de intenção de votos
* Estratificada: e quando a amostra é selecionada a partir de extratos da população. É usada quando se sabe que dentro da população, há uma desproporção entre grupos, mas se quiser ter certeza que haverá uma proporcionalidade na seleção da amostra

#### Medidas de Centralidade

* **Média**: diz a média dos dados em uma amostra. Sua fórmula é a soma de todos os dados da amostra divididos pela quantidade
* **Mediana**: diz qual o valor central em uma amostra. Seu cálculo é o valor central, em uma distribuição ímpar e a soma dos valores do meio numa distribuição par.

> A média e prejudicada se a distribuição não for tão normalizada, isto é, se haverem outliers (valores muito discrepantes), eles acabam jogando a média ou muito para cima ou muito para baixo. Fato que não ocorre com a mediana.

##### Medidas de Centralidade: Python

* Para a média, use *numpy.mean(list)*
* Para a mediana, use *numpy.median(list)*

#### Medidas de Variabilidade

* **Variância**: é a soma das diferenças dos valores em relação a média, dividido pela quantidade total menos 1. Ela e usada para saber qual a variação dos dados em minha amostra.
* **Desvio Padrão**: é a raiz quadrada da variância. Diz o valor médio de variação dos dados em relação a média.
* **Amplitude**: é a diferença absoluta entre o menor e maior valor na amostra.

##### Medidas de Variabilidade: Python

* Para o desvio padrão, use *numpy.std(list)*

#### Probabilidade

E a chance de um dado evento `E` acontecer em um número de experimentos `p`. O cálculo da probabilidade se resume a:

`E` dividido por `p`.

* **Eventos independentes**: significa que um próximo experimento é independente de algum outro. Exemplo: jogar uma moeda e dar cara.
* **Eventos dependentes**: significa que um experimento e influenciado por algum outro. Exemplo: qual a chance de eu retirar um Às de Copas de um baralho e depois um Reis de Copas.

Links:
* [Geekie Games](https://geekiegames.geekie.com.br/blog/probabilidade-condicional/)
* [Série de Aulas do Codecademy](https://geekiegames.geekie.com.br/blog/probabilidade-condicional/)

#### Distribuições

São formas de explicar dados aleatorios, de maneira que possamos encontrar um padrão e determinar comportamentos.

#### Distribuição Binomial

É uma distribuição que afirma que seus elementos só podem estar em duas condições, daí seu nome. Para se usar a distribuição binomial, é necessário cumprir certos pré-requisitos

* Número Fixo de Experimentos
* Cada experimento pode ter 2 resultados apenas: sucesso ou fracasso
* A probabilidade de sucesso deve ser a mesma em cada experimento
* Os experimentos são independentes

> Um exemplo de cenário para uso do cálculo de probabilidade usando a distribuição normal é o cálculo com moedas.

Links:
* [UFSC](https://www.inf.ufsc.br/~andre.zibetti/probabilidade/binomial.html)
* [IME](https://www.ime.usp.br/~yambar/MAE116-Quimica/Aula%205%20Distribui%E7%E3o%20Binomial/Aula%205%20-%20Distribui%E7%E3o%20Binomial.pdf)
* [UFRGS](http://www.producao.ufrgs.br/arquivos/disciplinas/489_estaind005_distprob.pdf)

#### Distribuição normal

É a distribuição mais conhecida. Ela é usada para cálculo da ocorrência de um valor dentro de uma determinada distribuição. Para tanto, essa distribuição precisa ser considerada normal.

Uma distribuição normal, é quando os itens estão dispostos de maneira assimétrica em relação a média dos dados. Um gráfico de uma distribuição normal se parece bastante com um sino

Links:
* [Voitto](https://www.voitto.com.br/blog/artigo/distribuicao-normal)
* [IME](https://www.ime.usp.br/~hbolfar/aula_2013/Aula6-A12012.pdf)
* [Portal Action](http://www.portalaction.com.br/probabilidades/62-distribuicao-normal)
* [USP](https://edisciplinas.usp.br/pluginfile.php/3993614/mod_resource/content/4/mineracaodadosbiologicos-parte2.pdf)

#### Intervalos de Confiança

Diz respeito a inferência de informações de uma população a partir de uma amostra. Imaginemos uma pesquisa eleitoral. Não é possível afirmar com 100% de certeza que um candidato vai ganhar a partir de uma simples pesquisa. Mas a partir de uma série delas, podemos chegar a conclusões, porém, entendendo que uma amostra, por mais seleta que seja, não é a população.

Links:
* [Portal Action](http://www.portalaction.com.br/inferencia/intervalo-de-confianca)

#### Testes de Hipótese

Como saber se uma hipótese levantada a partir de um conjunto de dados é correto? Como saber se uma pesquisa eleitoral é confiável?

Links:
* [Portal Action](http://www.portalaction.com.br/inferencia/51-introducao)

#### Correlação

É quando existe uma relação matemática entre duas variáveis. Exemplo: quando eu afirmo que, quanto maior a idade de um paciente, maior o valor médio investido para o tratamento de tal paciente, eu tenho que variáveis são valor investido e idade do paciente.

É importante entender que, quando temos uma correção temos dois tipos de variáveis: as **explanatórias** e as **dependentes**. Em que as explanatórias são as que explicam as dependentes. No caso acima, idade do paciente é uma variável explanatória e valor investido é dependente.

> Quando eu tenho uma relação forre entre as variáveis, eu consigo prever um valor de uma variável dependente, tendo como base o valor de uma variável explanatória. Base de estudo da Regressão Linear

#### Coeficiente de Determinação

É o coeficiente acima elevado ao quadrado. Mostra a porcentagem de quanto uma variável independente pode ser explicada pela explanatória.

#### Regressão Linear Simples e Múltipla

É quando eu prevejo um valor de uma variável dependente a partir de uma explanatória

Conceitos:
* **Residuais**: é a diferença entre uma variável qualquer e a reta que pode ser trassada numa dispersão de dados de uma regressão simples, isto é, a inclinação
* **Outliers**: são os dados que fogem muito do padrão

Tipos:

* Simples: tenho uma explanatória para uma dependente
* Múltipla: tenho duas ou mais explanatórias para uma dependente. Para tanto, cada variável explanatória precisa ser independentes entre si

Links:
* [EECIS](https://www.eecis.udel.edu/~portnoi/classroom/prob_estatistica/2006_2/lecture_slides/aula20.pdf)
* [IME](https://www.ime.usp.br/~fmachado/MAE229/AULA10.pdf)
