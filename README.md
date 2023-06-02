# Rede Geográfica com Algoritmos de Busca

Este é um projeto de exemplo que demonstra a criação de uma rede geográfica e a aplicação de diferentes algoritmos de busca nessa rede. O código utiliza a biblioteca NetworkX para criar e visualizar o grafo da rede, bem como implementa os algoritmos de busca em profundidade, busca em largura, busca Best-First e A*. 

## Pré-requisitos

Antes de executar o código, é necessário ter as seguintes bibliotecas instaladas:

- NetworkX
- Matplotlib
- ipywidgets

Você pode instalá-las utilizando o gerenciador de pacotes do Python, pip, da seguinte forma:

```
pip install networkx matplotlib ipywidgets
```

## Como executar o código

1. Certifique-se de ter as bibliotecas mencionadas acima instaladas corretamente.
2. Copie e cole o código em um arquivo Python com extensão `.py`.
3. Execute o arquivo Python em um ambiente que suporte as bibliotecas utilizadas.

## Descrição do código

O código é dividido em várias partes, cada uma responsável por uma etapa específica. A seguir, uma breve descrição de cada parte:

### Geração da Rede Geográfica

A função `gera_rede_geografica` é responsável por criar uma rede geográfica com base no número de vértices e no parâmetro lambda (λ). A rede geográfica é gerada utilizando coordenadas aleatórias para os vértices e a probabilidade de existir uma aresta entre dois vértices é calculada com base na distância euclidiana entre eles.

As funções `gera_vertices` e `gera_arestas` são utilizadas pela função `gera_rede_geografica` para criar a lista de vértices e a lista de arestas da rede geográfica, respectivamente.

### Visualização da Rede Geográfica

O código utiliza a biblioteca Matplotlib para visualizar a rede geográfica. A função `atualiza_grafo` é responsável por atualizar o grafo com base no valor de lambda (λ) fornecido. Essa função utiliza a função `gera_rede_geografica` para gerar uma nova lista de vértices e arestas, e então atualiza o grafo e o desenha utilizando a biblioteca NetworkX e a função `nx.draw_networkx`.

### Algoritmos de Busca

O código implementa quatro algoritmos de busca: busca em profundidade, busca em largura, busca Best-First e A*.

A função `busca_em_profundidade` realiza a busca em profundidade no grafo, buscando um caminho entre um vértice de origem e um vértice de destino. A função utiliza uma pilha para armazenar os vértices a serem explorados e um conjunto para marcar os vértices visitados.

A função `busca_em_largura` realiza a busca em largura no grafo, buscando um caminho entre um vértice de origem e um vértice de destino. A função utiliza uma fila para armazenar os vértices a serem explorados e um conjunto para marcar os vértices visitados.

A função `busca_best_first` realiza a busca Best-First no grafo, buscando um caminho entre um vértice de origem e um vértice de destino. A função utiliza uma fila de prior

A função `busca_best_first` realiza a busca Best-First no grafo, buscando um caminho entre um vértice de origem e um vértice de destino. A função utiliza uma fila de prioridade para armazenar os vértices a serem explorados, onde a prioridade é determinada pela heurística de proximidade ao vértice de destino.

A função `busca_a_estrela` realiza a busca A* no grafo, buscando um caminho entre um vértice de origem e um vértice de destino. A função utiliza uma fila de prioridade para armazenar os vértices a serem explorados, onde a prioridade é determinada pela soma do custo acumulado do caminho até o vértice e a heurística de proximidade ao vértice de destino.

### Execução do Código

Após definir os algoritmos de busca, o código permite a interação com o usuário através de widgets interativos. O usuário pode definir o número de vértices da rede geográfica, o valor de lambda (λ) que controla a probabilidade de existir uma aresta entre dois vértices, o vértice de origem e o vértice de destino para a busca.

Ao definir os parâmetros, o código irá gerar a rede geográfica, exibir o grafo e executar cada um dos algoritmos de busca, mostrando o caminho encontrado.

## Considerações Finais

Este projeto de exemplo demonstra a criação de uma rede geográfica e a aplicação de diferentes algoritmos de busca. É importante ressaltar que o código apresentado aqui é simplificado e tem como objetivo fornecer uma visão geral do processo. Para casos mais complexos, podem ser necessários ajustes e otimizações adicionais.

Você pode copiar e colar o código fornecido em um arquivo Python e executá-lo para visualizar a rede geográfica e testar os algoritmos de busca. Espero que isso seja útil! Se você tiver alguma dúvida adicional, sinta-se à vontade para perguntar.
