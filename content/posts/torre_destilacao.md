+++ 
draft = false
date = 2020-01-04T19:04:44-03:00
title = "Dimensionamento de coluna de destilação para separação de hidrocarbonetos obtidos a partir  da desoxigenação de Ácido oleico com catalisador aerogel"
description = ""
slug = "torre-de-destilacao" 
tags = ["engenharia química", "combustíveis renováveis", "catálise", "destilação"]
categories = []
externalLink = ""
series = []
author = "Rafael Belo Duarte"
toc = true
+++

*Rafael Belo Duarte (PIBIC/CNPq/FA/Uem), J. L. C. W. Pimenta, O. A. A. Santos (Coorientadora), L. M. M. Jorge (Orientador).*

*Universidade Estadual de Maringá / Centro de Tecnologia / Maringá, PR.*

*Área: Engenharia Química. Subárea: Operações industriais e equipamentos para Engenharia Química.*

## Resumo

Óleos vegetais podem ser utilizados como fonte de biomassa para a produção de combustíveis renováveis, os produtos obtidos a partir destes óleos têm baixa concentração de contaminantes e são potenciais substitutos a combustíveis obtidos a partir do petróleo. Neste trabalho, um catalisador aerogel, impregnado com carbetos de níquel e molibdênio, foi utilizado na produção de hidrocarbonetos a partir de óleo de soja, em um reator batelada. Os produtos da reação foram analisados, quantificados e, a partir dos resultados, dimensionou-se uma coluna de destilação para realizar a separação das várias frações de hidrocarbonetos parafínicos de acordo com suas temperaturas de ebulição.

[Topo](#top)

## Introdução

A substituição de combustíveis fósseis por alternativas renováveis é uma área que vem recebendo muita atenção nos últimos anos. Tais combustíveis alternativos, vêm de plantas, animais e microrganismos, que capturam seu carbono diretamente da atmosfera, devolvendo-o ao fim de seu ciclo de vida. Seu impacto ambiental é menor comparado aos combustíveis fósseis que, ao serem extraídos e utilizados, liberam uma carga de carbono que estava armazenada na crosta terrestre há milhões de anos.
As fontes de combustíveis renováveis, como o óleo de soja, por possuírem pequenas concentrações de enxofre, nitrogênio e metais pesados, são interresantes para a produção, por exemplo, de querosene de aviação, gasolina e diesel (Wang, 2012)[^fn].
 
Uma das restrições ao uso de combustíveis obtidos a partir de óleos vegetais, na forma de ésteres monoalquílicos é que, conforme a temperatura ambiente se aproxima do ponto de fusão, pequenos cristais de grandes moléculas saturadas começam a aparecer, o que pode causar o entupimento de componentes, como válvulas e tubulações (Pimenta, 2018)[^fn1]. 

Conforme o exposto, os objetivos deste trabalho são descrever como e em que condições foi realizada a reação de desoxigenação e, a partir da análise dos produtos, dimensionar uma coluna de destilação para separar os compostos de interesse.

[Topo](#top)

## Materiais e métodos

### Preparação da mistura de hidrocarbonetos a partir de óleo de soja

A reação foi realizada em batelada com um reator Parr, de aço inoxidável 316L, que possui volume de 300 mL, agitador mecânico do tipo turbina de pás retas inclinadas e válvulas para a retirada de amostras líquidas e gasosas.   Ao reator adicionou-se 25 g de óleo de soja e 0,5 g de catalisador sol-gel impregnado com carbetos de níquel e molibdênio. Selou-se o reator e foi feita uma purga com H2, mantendo a pressão atmosférica. Iniciou-se uma rampa de aquecimento até 380 ºC, com agitação constante de 800 rpm, atingida a temperatura de operação pressurizou-se o reator com hidrogênio até 50 bar, aqui considera-se o início da reação. Após 40 minutos foi retirada amostra líquida.

### Análise da amostra

Como desejava-se analisar a amostra em uma coluna cromatográfica, realizou-se uma metilação, para converter ácidos graxos livres, danosos à coluna de separação, em seus respectivos ésteres metílicos.
A amostra líquida foi analisada em um cromatógrafo da Agilent Technologies modelo 7890B, com coluna DB5-ms, com hélio como eluente. A corrida cromatográfica inicia-se em 50 ºC, com rampa de aquecimento de 8 ºC/min até 260 ºC. Os compostos foram identificados por um espectrômetro de massas e quantificados com um detector de ionização de chama.

### Dimensionamento da coluna de destilação

Utilizando-se o software ChemSep (versão 8) para a realização dos balanços de massa e energia, partiu-se de uma coluna com 16 estágios, vazão de produto de fundo de 415,86 Kmol/dia, razão de refluxo igual a 8, condensador parcial com retirada de produto na forma de vapor, um refervedor parcial com saída de produto líquido e saídas de 50% de vapor nos estágios 5 e 11, a alimentação entra no estágio 9 a 240,56 ºC. Defininiu-se um espassamento de 0,5 m entre os pratos. Não avaliou-se queda de pressão, portanto utilizou-se  pressão constante a 1 atm. 
Os produtos foram denominados de acordo com suas temperaturas de ebulição. Segundo Zandonai (2016)[^fn2], tem-se como gasolina o que está entre 36,85 e 176,85 ºC, querosene entre 176,85 e 245,85 ºC e diesel na faixa de 245,85 a 344,85 ºC, a uma pressão de 1 atm.

[Topo](#top)

## Resultados e Discussão

A análise da amostra revelou que a fração mais significativa do produto é composta por moléculas que possuem de 15 a 18 carbonos, com pequenas quantidades na faixa do C8 ao C10 e frações ainda menores do C11 ao C14. Tomou-se a composição desta amostra como alimentação, que pode ser observada na Tabela 1, para o dimensionamento de uma  coluna de destilação.

Os produtos retirados da coluna foram classificados de acordo com a faixa de temperatura, como na Figura 1. No topo temos uma mistura com temperatura de ebulição de 137,54 ºC, que foi classificada como gasolina leve, nos estágios 5 (Gasolina) e 11 (Querosene) retira-se vapor saturado a 157,47 ºC e 243,10 ºC, respectivamente.

![coluna](/images/coluna.png "Figura 1 –  Coluna de destilação.")

A eficiência dos pratos é estimada utilizando-se a correlação de O’Connell, de maneira iterativa, que fornece uma eficiência média de 0,3961. As cargas térmica no condensador e refervedor são -19 490,3 J/s e 203 205 J/s, nesta ordem.

Como o espassamento entre os pratos é de 0,5 m, a altura da coluna é 7,5 m. O diâmetro depende das vazões utilizadas e foi calculado baseado na velocidade de inundação para o vapor, obteve-se 21 cm para a seção de retificação (estágios 2 ao 8) e 44 cm para a seção de exaustão (estágios 9 ao 15).

Os resultados da Tabela 1, abaixo, sugerem que a partir da coluna descrita acima é possível obter gasolina, querosene e óleo diesel.

*Tabela 1 – Composições das correntes na coluna de destilação em frações molares.*

|  			Componente 		     |  			Alimentação 		     |  			Gasolina 			Leve 		        |  			Gasolina 			 			 		           |  			Querosene 			 			 		           |  			Diesel 		     |
|--------------    |---------------    |-----------------       |--------------          |---------------          |----------    |
|  			C8 		     |  			0,0350 		     |  			0,7310 		     |  			0,3307 		     |  			0,1930 		     |  			0,0005 		     |
|  			C9 		     |  			0,0350 		     |  			0,2284 		     |  			0,3607 		     |  			0,2366 		     |  			0,0030 		     |
|  			C10 		     |  			0,0250 		     |  			0,0368 		     |  			0,1896 		     |  			0,1609 		     |  			0,0080 		     |
|  			C11 		     |  			0,0090 		     |  			0,0025 		     |  			0,0349 		     |  			0,0424 		     |  			0,0057 		     |
|  			C12 		     |  			0,0200 		     |  			0,0010 		     |  			0,0315 		     |  			0,0592 		     |  			0,0174 		     |
|  			C13 		     |  			0,0200 		     |  			0,0002 		     |  			0,0128 		     |  			0,0367 		     |  			0,0197 		     |
|  			C14 		     |  			0,0090 		     |  			0,0000 		     |  			0,0024 		     |  			0,0100 		     |  			0,0094 		     |
|  			C15 		     |  			0,0490 		     |  			0,0000 		     |  			0,0066 		     |  			0,0353 		     |  			0,0527 		     |
|  			C16 		     |  			0,1190 		     |  			0,0000 		     |  			0,0087 		     |  			0,0559 		     |  			0,1302 		     |
|  			C17 		     |  			0,2390 		     |  			0,0000 		     |  			0,0102 		     |  			0,0746 		     |  			0,2642 		     |
|  			C18 		     |  			0,4400 		     |  			0,0000 		     |  			0,0120 		     |  			0,0953 		     |  			0,4891 		     | 			0,4891 		 |

[Topo](#top)

## Conclusões

Os produtos obtidos a partir da reação descrita são semelhantes aos hidrocarbonetos encontrados no petróleo, portanto, o processo se demonstra como uma alternatíva viável.  A separação dos produtos na coluna de destilação se mostra simples, o que diminui os custos de separação.

## Agradecimentos

Agradecemos ao CNPq e Fundação Araucária pelo apoio financeiro ao desenvolvimento da pesquisa e ao COMCAP UEM pelo suporte técnico nas análises.

[Topo](#top)

## Referências

[^fn]: WANG, H. **Biofuels production from hydrotreating of vegetable oil using supported noble metals, and transition metal carbide and nitride.** 2012. 134f. Tese (Doutorado) – Programa de Pós-Graduação em Engenharia Química, Wayne State University, Detroit, Michigan, 2012.

[^fn1]: PIMENTA, J. **Síntese e avaliação de catalisador não convencional na produção de hidrocarbonetos a partir do óleo de soja.** 2018. 130f. Dissertação (Mestrado) – Programa de Pós-Graduação em Engenharia Química, Universidade Estadual de Maringá, Maringá, Paraná, 2018.

[^fn2]: CASTELLÃ-PERGHER, S. FERNANDES-MACHADO, N.   SCALIANTE, M. YASSUE-CORDEIRO, P. ZANDONAI, C. **Production of petroleum-like synthetic fuel by hydrocracking of crude soybean oil over ZSM5 zeolite – Improvement of catalyst lifetime by ion exchange.** Fuel. v. 172, p. 228-237, 2016.
