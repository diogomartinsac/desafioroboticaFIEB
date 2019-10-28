Desafio de Robótica
===================

O quadricóptero autônomo deve procurar uma caixa preta no labirinto desviando de paredes e obstáculos. Para realizar a tarefa, foram adicionados 4 lasers, responsáveis por medir a distância até as paredes, e 4 sensores de visão, necessários para identificação da caixa. O mapa é discretizado de acordo com o intervalo escolhido e cada posição na matriz "mapMatrix" representa uma região do mapa. A matriz é inicializada e preenchida de acordo com leitura dos sensores e movimentação do veículo.

A "mapMatrix" pode ser preenchida com os seguintes valores:

Região desconhecida: 9

Parede:3

Posição atual:1

Região visitada:2

Região Livre: 0

Estratégia
==========

## Busca em Profundidade combinada com A* ##

A Busca em profundidade percorre as regiões livres(0) partindo da posição atual(1) e tem como objetivo encontrar uma região desconhecida(9). Essa informação alimenta o algoritmo de planejamento de trajetória (A*) responsável por entregar, se possível, o caminho a ser percorrido.

## Busca em Profundidade ##

A Busca em profundidade é utilizada para os casos em que o A* não consegue encontrar uma solução em alguma região.



