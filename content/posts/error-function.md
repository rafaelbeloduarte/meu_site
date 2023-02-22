+++ 
draft = false
date = 2021-03-16T01:00:43-03:00
title = "Fenômenos de transporte: Função erro de Gauss e a transferência de calor em regime transiente"
description = ""
slug = "funcao-erro" 
tags = ["engenharia química", "fenômenos de transporte"]
categories = []
externalLink = ""
series = []
+++

A função erro de Gauss (Equação \ref{eq1}) aparece quando se deseja resolver problemas de transferência de calor em regime transiente.

$$
erf(x) = \frac{2}{\sqrt{\pi}} \int{e^{-x^2}} dx
\label{eq1} \tag{1}
$$

A função erro complementar é:

$$
erfc(x) = 1 - erf(x)
\label{eq2} \tag{2}
$$

Um exemplo de sua utilização é na solução da equação do calor para um sólido seminfinito.

$$
\frac{\partial^2{T}}{\partial{x^2}} = \frac{1}{\alpha} \frac{\partial{T}}{\partial{t}} 
\label{eq3} \tag{3}
$$

**T** é a temperatura, **x** o comprimento (de uma placa ou profundidade do solo por exemplo), **$\alpha$** é a difusividade térmica e **t** o tempo. A solução dessa equação envolve a utilização de uma variável similar $ \eta \equiv \frac{x}{{4 \alpha t}^{1/2}} $. São calculadas as derivadas de $ \eta $ e substitui-se na Equação \ref{eq3}. Após a mudança de variável a equação diferencial parcial é transformada em equação diferencial ordinária que, ao ser integrada, solicita a solução da integral da Equação \ref{eq1}. A solução da Equação \ref{eq3} é: 

$$
\frac{T(t)-T_s}{T_i-T_s} \equiv erf (\eta)
\label{eq4} \tag{4}
$$

Onde **T(t)** é a temperatura no tempo **t**, **$T_s$** a temperatura da superfície (*constante e diferente da temperatura inicial*) e **$T_i$** a temperatura inicial.

O desenvolvimento, condições de contorno utilizadas e tabela com os valores das funções **erf(x)** e **erfc(x)** são apresentados em detalhes por Incropera [^fn1].

## Referências

[^fn1]: Incropera, Frank P. DeWitt, David P. Bergman, Theodore L. Lavine, Adrienne S. Fundamentos de Transferência de Calor e Massa. 2008, 6ª ed. LTC: Rio de Janeiro, RJ. 










