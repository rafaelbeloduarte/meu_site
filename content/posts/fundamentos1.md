+++ 
draft = false
date = 2021-01-31T18:03:43-03:00
title = "Fundamentos: equação geral dos balanços de massa"
description = ""
slug = "fundamentos-parte1"
tags = ["fundamentos da engenharia química", "engenharia química"]
categories = []
externalLink = ""
series = []
+++

## Equação geral dos balanços de massa

A Equação 1 ilustra um dos conceitos mais fundamentais da engenharia química. Ela surge quando se toma um certo volume definido no espaço onde deseja-se contabilizar entradas, saídas e acúmulo de matéria, e é aplicada em uma região do espaço onde define-se uma fronteira, real ou imaginária, que pode ser um equipamento industrial, uma planta química inteira ou qualquer outra região do universo.

$$
entrada + geração - saída - consumo = acúmulo
\tag{1} 
$$

É importante notar que os termos de geração e consumo na Equação 1 não supõem geração de matéria, pois isso viola o princípio da conservação de massa. Eles são úteis quando estuda-se sistemas com reações químicas e representam as transformações em quantidade de matéria. Por exemplo, quando surge uma molécula (geração), isto ocorre apenas a partir do consumo de outras espécies químicas, e o contrário é verdadeiro para o consumo.

Portanto, podem ser escritas diversas equações para um sistema, como uma equação para cada componente químico. Obtém-se então um sistema de [equações lineares](https://brasilescola.uol.com.br/matematica/equacao-linear.htm) (sistemas de equações não lineares é um bicho bem mais cabeludo), que pode ser resolvido caso o número de variáveis desconhecidas seja igual ao número de equações independentes, ou seja, o grau de liberdade (GL) é zero.

$$
graus\ de\ liberdade = número\ de\ variáveis - número\ de\ equações\ independentes
\tag{2} 
$$

Sistemas com graus de liberdade menor que zero não possuem solução, e em sistemas com graus de liberdade maior que zero existem infinitas soluções e devem ser feitas suposições até que tenha-se GL = 0.

## Referências

Felder, R. M. e Rousseau, R. W., 2005. Elementary principles of chemical processes. Wiley, Hoboken, NJ.

Himmelblau, D. M. e Riggs, J. B., 2004. Basic principles and calculations in chemical engineering. Prentice Hall PTR/Pearson, Upper Saddle River, NJ.
