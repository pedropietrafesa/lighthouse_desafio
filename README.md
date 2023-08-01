# Precificação de Veículos 

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

Para responder as perguntas do cliente, testar as hipóteses levantadas e precificar os carros o projeto utilizou análise de dados descritiva, com medidas de tendência central, de variância e correlações para as variáveis numéricas. No caso das variáveis categóricas, tabelas de frequência. No caso da visualização dos dados foram utilizados histogramas, gráficos de barras, boxplots, gráficos de dispersão,  lollipop e de distribuição dos valores faltantes por coluna. Nos testes hipóteses, Mann–Whitney e ANOVA  

(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- etc. (be as specific as possible)

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](link)
* [Notebook/Markdown/Slide DeckTitle](link)
* [Blog Post](link)


## Contributing DSWG Members

**Team Leads (Contacts) : [Full Name](https://github.com/[github handle])(@slackHandle)**

#### Other Members:

|Name     |  Slack Handle   | 
|---------|-----------------|
|[Full Name](https://github.com/[github handle])| @johnDoe        |
|[Full Name](https://github.com/[github handle]) |     @janeDoe    |

## Contact
* If you haven't joined the SF Brigade Slack, [you can do that here](http://c4sf.me/slack).  
* Our slack channel is `#datasci-projectname`
* Feel free to contact team leads with any questions or if you are interested in contributing!
