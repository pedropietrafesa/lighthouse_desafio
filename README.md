# Precificação de Veículos 

[![NPM](https://img.shields.io/npm/l/react)](https://github.com/pedropietrafesa/lighthouse_desafio/blob/main/LICENSE)

Este trabalho fez parte do desafio para Cientistas de Dados do projeto Lighthouse 2023-9 da [Indicium](https://indicium.tech).

#### Status do Projeto: [Completo]

## Objetivo do Projeto

O objetivo do projeto é criar um modelo preditivo que precifique os carros do cliente, que possui uma empresa de compra e venda de veículos usados, de forma que os preços fiquem o mais próximo possível dos valores de mercado.

Para alcançar o objetivo proposto, analisamos os dados disponibilizados por empresa de marketplace para compreender o mercado nacional, bem como para responder perguntas de negócio do cliente e apresentar modelo de predição.

### Parceiros
* [Indicium](https://indicium.tech)

### Métodos Utilizados 
* Machine Learning
* Análise Exploratória dos Dados (EDA)
* Modelos de Predição 
  
### Tecnologias
* Python
   
## Descrição do Projeto 

A base de dados trabalhada no projeto foi desenvolvida por empresa de marketplace com 29 colunas, sendo 28 de variáveis _features_ e a variável _target_, preço dos veículos anunciados. A seguir segue o dicionário dos dados.

* **id:** Contém o identificador único dos veículos cadastrados na base de dados
* **num_fotos:** contém a quantidade de fotos que o anuncio do veículo contém
* **marca:** Contém a marca do veículo anunciado
* **modelo:** Contém o modelo do veículo anunciado
* **versao:** Contém as descrições da versão do veículo anunciando. Sua cilindrada, quantidade de válvulas, se é flex ou não, etc.
* **ano_de_fabricacao:** Contém o ano de fabricação do veículo anunciado
* **ano_modelo:** Contém o modelo do ano de fabricação do veículo anunciado
* **hodometro:** Contém o valor registrado no hodômetro do veículo anunciado
* **cambio:** Contém o tipo de câmbio do veículo anunciado
* **num_portas:** Contém a quantidade de portas do veículo anunciado
* **tipo:** Contém o tipo do veículo anunciado. Se ele é sedã, hatch, esportivo, etc.
* **blindado:** Contém informação se o veículo anunciado é blindado ou não
* **cor:** Contém a cor do veículo anunciado
* **tipo_vendedor:** Contém informações sobre o tipo do vendedor do veículo anunciado. Se é pessoa física (PF) ou se é pessoa jurídica (PJ)
* **cidade_vendedor:** Contém a cidade em que vendedor do veículo anunciado reside
* **estado_vendedor:** Contém o estado em que vendedor do veículo anunciado reside
* **anunciante:** Contém o tipo de anunciante do vendedor do veículo anunciado. Se ele é pessoa física, loja, concessionário, etc
* **entrega_delivery:** Contém informações se o vendedor faz ou não delivery do veículo anunciado
* **troca:** Contém informações o veículo anunciado já foi trocado anteriormente
* **elegivel_revisao:** Contém informações se o veículo anunciado precisa ou não de revisão
* **dono_aceita_troca:** Contém informações se o vendedor aceita ou não realizar uma troca com o veículo anunciado
* **veiculo_único_dono:** Contém informações o veículo anunciado é de um único dono
* **revisoes_concessionaria:** Contém informações se o veículo anunciado teve suas revisões feitas em concessionárias
* **ipva_pago:** Contém informações se o veículo anunciado está com o IPVA pago ou não
* **veiculo_licenciado:** Contém informações se o veículo anunciado está com o licenciamento pago ou não
* **garantia_de_fábrica:** Contém informações o veículo anunciado possui garantia de fábrica ou não
* **revisoes_dentro_agenda:** Contém informações se as revisões feitas do veículo anunciado foram realizadas dentro da agenda prevista
* **veiculo_alienado:** Contém informações se o veículo anunciado está alienado ou não
* **preco (target):** Contém as informações do preço do veículo anunciado

O cliente levantou três questões para analisar nomerca revenda de automóveis, foram elas: 

* Qual o melhor estado cadastrado na base de dados para se vender um carro de marca popular e por quê?
* Qual o melhor estado para se comprar uma picape com transmissão automática e por quê?
* Qual o melhor estado para se comprar carros que ainda estejam dentro da garantia de fábrica e por quê?

Algumas hipóetes foram levantandas no decorrer da análise exploratória dos dados:

* Carros de marcas de luxo com alta quilometragem e data de fabricação acima de dez anos tem preço médio similar a carro de marca popular semi novo.
* Os carros anunciados em cidades do interior e que já foram trocados anteriormente são mais caros em média do que os da capital.
* Há diferença média de preços nos carros das marcas populares para as cores branco, prata e preto.

Para responder as perguntas do cliente, testar as hipóteses levantadas e precificar os carros o projeto utilizou análise de dados descritiva, com medidas de tendência central, de variância e correlações para as variáveis numéricas. No caso das variáveis categóricas, tabelas de frequência. No caso da visualização dos dados foram utilizados histogramas, gráficos de barras, boxplots, gráficos de dispersão,  lollipop e de distribuição dos valores faltantes por coluna. Nos testes hipóteses, Mann–Whitney e ANOVA foram empregados para verificar se ocorreu diferenças significativas das médias entre duas, ou entre três ou mais amostras. Na proposta do melhor modelo de precificação foram testados, regressão linear, _Random Forest_, _Gradient Boosting_, _Extra Trees Regressor_ e XGBoost.

Dois desafios o banco de dados nos trouxe. O primeiro, oito variáveis _features_, categóricas, com mais de 25% de dados faltantes. O segundo, três variáveis _features_ com mais de 400 categorias, sendo que a variável "versões" possui 1916 diferentes categorias.  


## Requisitos deste projeto

- Análise Descritiva/Análise Exploratória (EDA)
- Limpeza dos Dados 
- Modelagem Estatística
- Relatório

## Getting Started

1. Caso deseje, há a possibilidade de clonar este repositório (veja [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. O download do banco de dados de treino pode ser realizado neste ([link](https://raw.githubusercontent.com/pedropietrafesa/lighthouse_desafio/main/cars_train.csv)).
3.  O download do banco de dados de teste pode ser realizado neste ([link](https://raw.githubusercontent.com/pedropietrafesa/lighthouse_desafio/main/cars_test.csv)).
    
4. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
5. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](link)
* [Notebook/Markdown/Slide DeckTitle](link)
* [Blog Post](link)


## Membro do Projeto

**(Contato) : [Pedro Araújo Pietrafesa](https://github.com/[pedropietrafesa])(@pedropietrafesa)**



