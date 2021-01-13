# Projeto 1 - Insights

Projeto que cobre questão de negócio, o entendimento do negócio, a coleta de dados, a limpeza de dados e a exploração de dados.

## Programas utilizados: 
- Visual Studio Code
- Python(Pandas, Matplotlib e Numpy)
- Jupyter Notebook 

## Dados utilizados: 
https://www.kaggle.com/harlfoxem/housesalesprediction
Esse conjunto de dados contém casas vendidas entre Maio de 2014 e Maio de 2015. Você usará esses dados para desenvolver sua solução.

## Contexto do projeto - Dia 1: 
A House Rocket é uma plataforma digital que tem como modelo de negócio, a compra e a venda de imóveis usando tecnologia.

Você é um Data Scientist contrato pela empresa para ajudar a encontrar as melhores oportunidades de negócio no mercado de imóveis. O CEO da House Rocket gostaria de maximizar a receita da empresa encontrando boas oportunidades de negócio.

Sua principal estratégia é comprar boas casas em ótimas localizações com preços baixos e depois revendê-las posteriormente à preços mais altos. Quanto maior a diferença entre a compra e a venda, maior o lucro da empresa e portanto maior sua receita.

Entretanto, as casas possuem muitos atributos que as tornam mais ou menos atrativas aos compradores e vendedores e a localização também pode influenciar os preços.

- Quais casas o CEO da House Rocket deveria comprar e reformar para aumentar o preço de venda? 
- Quais seriam as sugestões de mudanças? 
- Qual o incremento no preço dado pela reforma? 

## Roteiro - Dia 1: 
- Limpeza e organização do arquivo 
- Analise dos dados
- Filtar os arquivos com base na analise feita 

## Resposta - Dia 1: 
Dividi as prioridades de compra em 3 categorias: Principal, Segunda e Terceira,
- As principais casas que o CEO deveria comprar são as de ID: 2322029048, 2220069003. Com a ampliação dos espaços de vivencia e adições de 3 quartos e 4 banheiros. As casas terão um aumento no valor atual de no mínimo 400% (x4).
- As de segunda prioridade, ID: 2724079090 e 1125079111, possuem um valor base maior que as primeiras, o que dificulta o potencial aumento delas. As casas precisam de uma ampliação dos espaços de vivencia, adição de 2 quartos, 5 e 3 banheiros, respectivamente e a construção de um porão. As casas terão um aumento no valor atual de no mínimo 300%(x3).
- As de terceira prioridade, ID: 722069232, 3626079040, 2522029039, 2624089007, 2623069031, 2323089009, 225079036, 619079096, 822039004, 522079022, 1623089165, são casas com grande disponibilidade de construção de áreas de vivencia, mas possuem problemas como preço base atual, condições de contrato ou necessidade de uma grande reforma na decoração. Mas uma base para a reforma é no mínimo a adição de 2 quartos, 4 banheiros e ampliação ou construção de porões. O incremento no preço das casas pode varias de no mínimo 200%(x2) até 400%(x4).

 
## Contexto do projeto - Dia 2:
3 clientes distintos apareceram na corretora e estipularam os detalhes que gostariam de encontrar numa casa 

- Paulo gostaria de encontrar uma casa com 5 quartos, 3 banheiros, 2 andares e 2 pontos de vista
- Gabriel gostaria de uma casa que custasse menos de 550.000,00 e possua 4 quartos, 2 banheiros, 1 andar, 3 pontos de vista e construida ou reformada depois do ano de 2005 
- Henrique deseja uma casa que custe menos de 350.000,00 e possua 2 quarto, 2 banheiros, 1 andar, 3 pontos de vista e construida ou reformada  entre 1990 e 2010

## Roteiro - Dia 2: 
- Filtrar o arquivo com base nas necessidades do cliente 

## Resposta - Dia 2:
- Em nosso sistema só foi encontrado uma casa que atenda todos os requisitos perfeitamente de Paulo e 5 outras que possuem 3 ou 4 pontos de vista . A casa de ID: 9523104345, que custa 825.000,00 dolares, é a que atende todos os requisitos de Paulo
- Foi encontrado a casa de ID: 2309710130, que custa 272.000,00 dolares. 
- Encontramos 2 casas que atendem os requisitos perfeitamente de Henrique. As casas de ID: 5702450250 e 8141300030, com o mesmo valor de 340.000,00      

## Graficos 
| Porcentagem de banheiros construidos nas casas | Porcentagem das atrações disponiveis perto das casas |
|-|-|
|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico1.png" width="500" height="500" />|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico2.png" width="500" height="500" />|

| Outros (Atrações) | Casas construidas e reformadas |
|-|-|
|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico3.png" width="500" height="500" />|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico4.png" width="500" height="500" />|

| Casas construidas | Casas construidas |
|-|-|
|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico5.png" width="500" height="500" />|<img src="https://github.com/mathnr7/Projeto-1-Insights/blob/main/Graficos/Grafico6.png" width="500" height="500" />|

### Analise
- Casas que valem mais de 2 milhoes ja possuem uma quantidade base de dinheiro muito alta, assim prejudicando qualquer tipo de reforma ou reestruturação dela.
- Quanto maior o numero do sqft_lot melhor é local para uma reforma, mas lembrando que o numero de pontos de vista influencia bastante e o preço base também 
- A diferença entre 1 ponto de vista para 2 pontos de vista gera um aumento consideravel no preço da casa
- Quanto maior for o sqft_living maior vai ser a influencia do sqft_basement no valor da casa
- O waterfront não tem uma influencia consideravel em casas de valor baixo ou com uma quantidade de banheiros/quartos baixo 

License
----

MIT
