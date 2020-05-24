+++ 
draft = false
date = 2020-03-26T18:32:38-03:00
title = "Esterilização, desinfecção e proteção contra patógenos"
description = ""
slug = "esterilizacao-desinfeccao" 
tags = ["engenharia química", "bioquímica"]
categories = []
externalLink = ""
series = []
math = true
+++

É importante fazer a distinção entre **esterilização e desinfecção**. A primeira se refere à eliminação de todos os vírus e formas de vida em um meio ou superfície, já **a desinfecção não requer a completa destruição dos elementos contaminantes**, apenas uma fração, de acordo com o nível de assepsia que se deseja. Sempre que possível, deve-se trabalhar com técnicas que sejam capazes de inibir a propagação de agentes contaminantes após realizada a desinfecção e, principalmente, a esterilização.

Os agentes de desinfecção/esterilização podem ser classificados como químicos ou físicos, dependendo de seu mecanismo de ação. Entre os físicos temos o calor úmido (vapor) ou calor seco, radiação UV e radiação ionizante. Os agentes químicos incluem, por exemplo, o óxido de etileno, glutaraldeído e o bem conhecido etanol.[^fn1]

A recente crise de saúde pública causada pelo Covid-19 trouxe à superfície a necessidade de conter e isolar o vírus, que dissemina-se a partir do contato direto com pessoas infectadas ou por proximidade com estas, já que **partículas virais podem ser expelidas do corpo do vetor carregadas por pequenas gotículas de água, muco ou sólidos.** Por isso a importância de barreiras físicas, como **máscaras**, que apesar de possuírem canais e orifícios centenas ou milhares de vezes maiores que as partículas virais, ainda assim são capazes de capturá-las pois são materiais formados por emaranhados de fibras, onde eventualmente **as partículas contaminadas colidem e perdem sua energia cinética, ficando presas à superfície fibrosa por ação mecânica ou eletrostática.**

Quanto à desinfecção de superfícies, o Centro para Controle e Prevenção de Doença Infecciosas dos Estados Unidos (CDC), informa que a transmissão do Covid-19 ocorre principalmente através do ar, em gotículas e aerossóis, mas sabe-se que **o vírus pode permanecer viável em uma variedade de materiais por horas ou até dias.**[^fn2]

**A higienização de superfícies pode ser realizada com solução de álcool 70º INPM ou solução de hipoclorito de sódio com 0,1% (1000 ppm) de cloro ativo** ([^fn3],[^fn4]) (essa porcentagem é mássica e refere-se à quantidade de cloro ativo em certa quantidade de solução). Deve-se ter cuidado com o hipoclorito de sódio pois é um agente oxidante, corrosivo e branqueador e pode danificar certos materiais como tecidos, metais e até certos polímeros como o policarbonato.

A preparação de solução de álcool 70º INPM pode ser realizada de maneira muito simples com uma balança e qualquer álcool comercial com fração superior a 70º INPM. Requer-se apenas a diluição do álcool em água até obter-se a concentração desejada.

Sabendo que a escala INPM é mássica, tomemos como exemplo a preparação de solução alcoólica 70º INPM a partir de álcool 94º INPM. Sabemos que a fração mássica de etanol na solução mãe ($m_1$) é 0,94, então se partirmos de 1 Kg de solução temos:

$$
m_{etanol} = 0,94*1 Kg = 0,94 Kg
$$

Como na solução filha ($m_2$) a fração de etanol dever ser 0,70:

$$
0,70 = \frac{ m_{etanol} } { m_2 }
$$

$$
0,70 = \frac{ 0,94 Kg } { m_2 }
$$

$$
m_2 = \frac{0,94 Kg}{0,70} = 1,34 Kg
$$

Portanto, a diferença entra a massa da solução mãe e filha é a quantidade de água que devemos adicionar para atingir a concentração 70º INPM:

$$
m_{água-a-adicionar} = m_2 - m_1 = 1,34 Kg - 1 Kg = 340 g
$$

Dessa maneira, adicionando-se 340 g de água a 1 Kg de solução 94º INPM obtém-se 1,34 Kg de álcool 70º INPM. A razão pela qual soluções etanol-água (70º INPM é a concentração ótima) são mais efetivas que etanol anidro contra agentes patológicos está no fato de que **o principal mecanismo de ação microbiana do etanol é a desnaturação de proteínas, e estas são mais rapidamente desnaturadas na presença de água**[^fn3], que também diminui a volatilidade da solução e evita a rápida evaporação do etanol, aumentando o tempo de contato. A adição de agentes tensoativos às soluções alcoólicas também é realizada em alguns casos, pois muitos patógenos têm camadas lipídicas que são destruídas pela ação de detergentes, a redução da tensão superficial também contribui para a remoção mecânica de partículas contaminadas.

*Observação 1: Quando trabalhar com grandes volumes **realizar a adição lentamente, a diluição etanol-água é um processo exotérmico**, libera calor devido à energia liberada por ocasião da formação de ligações de hidrogênio. Por isso também, utilizamos massa ao invés de volumes para tomar nossas medidas, a solução água-etanol desvia-se muito da idealidade e apresenta diminuição de volume quando são misturados, devida em grande parte às já mencionadas ligações de hidrogênio.*

*Observação 2:* ***etanol é inflamável***, *manusear com cuidado, longe de fontes de ignição, em local bem ventilado e tendo em mente a Observação 1.*


A obtenção de álcool 70º INPM a partir de soluções menos concentradas só é possível por processos de destilação (pode ser simples) ou extração.

**Soluções com 0,1% cloro ativo podem ser preparadas a partir de água sanitária**, as comerciais geralmente têm 2% a 2,5% cloro ativo. Partindo da equação abaixo:

$$
C_1  V_1 = C_2  V_2
$$

Com C = concentração e V = volume.

Deseja-se produzir 5 L de solução 0,1% a partir de solução 2%, fazemos:

$$
2 \\% * V_1 = 0,1 \\% * 5 L
$$

E encontramos $V_1 = 0,25 L = 250 mL$. Portanto, **para preparar 5 L de solução desinfetante de hipoclorito, precisamos de 250 mL de solução 2% (água sanitária comercial), que deve ser completada com água até atingir 5 L.** Ou seja, 1 parte de água sanitária para 19 partes de água[^fn4].

# Referências

[^fn1]: Schmidell, W. Lima, U. A. Aquarone, E. Borzani, W. **Biotecnologia Industrial - Engenharia Bioquímica.** Volume 2. São Paulo: Blucher, 2001.

[^fn2]: **Environmental Cleaning and Disinfection Recommendations.** Centers for Disease Control and Prevention. U.S. Department of Health & Human Services. Disponível em: https://www.cdc.gov/coronavirus/2019-ncov/community/organizations/cleaning-disinfection.html. Acesso em: 26 de março de 2020.

[^fn3]: **Chemical Disinfectants.** Centers for Disease Control and Prevention. U.S. Department of Health & Human Services. Disponível em: https://www.cdc.gov/infectioncontrol/guidelines/disinfection/disinfection-methods/chemical.html. Acesso em: 26 de março de 2020.

[^fn4]: **Environmental cleaning and disinfection principles for COVID-19.** Department of Health. Australian Government. Disponível em: https://www.health.gov.au/sites/default/files/documents/2020/03/environmental-cleaning-and-disinfection-principles-for-covid-19.pdf. Acesso em: 26 de março de 2020.
