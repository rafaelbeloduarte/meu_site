+++ 
draft = false
date = 2022-08-18T15:21:04-03:00
title = "O Problema das Portas"
description = ""
slug = "problema-das-portas" 
tags = ["estatística", "probabilidade"]
categories = []
externalLink = ""
series = []
author = "Rafael"
+++

O livro "The Drunkards Walk" [^fn1] trata de como a aleatoriedade influencia nossas vidas e das dificuldades que as pessoas têm em entender probabilidade.

Em uma das passagens, para ilustrar esse último ponto, o autor traz o seguinte problema:

Imagine que é lhe dada uma escolha entre 3 portas, atrás de uma das portas há um prêmio e nas outras 2 nada.

Depois que você fez a escolha uma das portas onde não há nada é aberta e é lhe dada a escolha de trocar ou não de porta.

O que é mais vantajoso? Trocar ou não trocar? Ou não faz diferença?

Meu primeiro instinto, como o das maioria das pessoas segundo o autor, é que não importa se eu trocar ou não, agora nós temos apenas duas portas e minha probabilidade de ganhar é 1/2.

Mas isso não é verdade, a probabilidade de ganhar se eu trocar de porta é 2/3! Enquanto que se eu não trocar, continuo com a probabilidade inicial de 1/3.

# Por quê?

Pois quando foi me revelada uma das portas, eu possuo uma informação adicional e meu espaço de possibilidades mudou. Antes era a escolha aleatória entre as 3 portas, agora é a escolha entre trocar ou não de porta. São duas escolhas DIFERENTES.

A segunda escolha pode ser feita respondendo a seguinte pergunta: qual a probabilidade de escolher a porta errada? É 2/3. Dessa forma, 2/3 das vezes será escolhida a porta errada e nessas vezes será vantajoso trocar de porta.

Podemos experimentar com o problema usando o seguinte algoritmo:

1. Gerar uma lista aleatória, digamos que `0` são as portas vazias e `1` é o prêmio;
1. Escolhemos uma porta (um índice da lista) de maneira aleatória;
1. Removemos uma das portas vazias (um `0` qualquer);
1. Trocamos nossa escolha;
1. Repetimos `n` vezes sempre somando o `resultado` de nossa escolha aos anteriores;
1. Dividimos a soma por `n`.

Isso nos dará a proporção de sucessos. Em `python` podemos escrever o código abaixo. Iterando 1 milhão de vezes, a proporção é muito próxima a 2/3: 0,667355.

```
import random

n = 1000000
resultado = 0

for i in range(1, n):
    lista = [0,0,1]
    # embaralhar a lista
    random.shuffle(lista)
    
    # escolher uma porta
    escolha = random.choice(lista)
    
    # remover 1 zero (porta sem o prêmio)
    lista.remove(0)
    # trocar a escolha
    indice = lista.index(escolha)
    if indice == 0:
        indice = 1
    else: indice = 0
    
    # salvar o resultado
    resultado = resultado + lista[indice]

# calcular a proporção de sucessos
prop = resultado/n
print("#######################")
print("")
print("Proporção de sucessos = ", prop)
print("")
print("#######################")
```

## Referências

[^fn1]: Mlodinow, Leonard, 1954-. The Drunkard's Walk : How Randomness Rules Our Lives. New York :Pantheon Books, 2008.
