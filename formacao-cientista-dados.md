# Formação Cientista de Dados - Udemy

Esté um arquivo de resumo com todos os conteúdos e links que serviram de estudo no curso de Formação em Cientista de Dados da Udemy([Link](https://www.udemy.com/cientista-de-dados/))

## Roadmap do curso

## Estatistica
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

