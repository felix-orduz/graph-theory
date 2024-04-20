# Manual de Teoría de Grafos con SageMathCell y Phython

Este documento proporciona una guía paso a paso sobre cómo crear y manipular grafos utilizando SageMathCell, un recurso en línea para la computación matemática, especialmente útil para estudiantes y profesionales en el campo de la Teoría de Grafos. A continuación, se detallan los métodos para construir grafos simples, grafos con vértices nombrados individualmente y grafos con múltiples aristas entre el mismo par de vértices, como en el famoso problema de los puentes de Königsberg.

```python
# Importar la librería de grafos
G = Graph()

# Agregar vértices al grafo
G.add_vertices([0, 1, 2, 3])

# Agregar aristas al grafo
G.add_edges([(0, 1), (1, 2), (2, 3), (3, 0), (0, 2)])

# Dibujar el grafo
G.show()
```

Crear un Grafo nombrando uno por uno los elementos
```python
# Importar la librería de grafos
G = Graph()

# Agregar vértices al grafo
G.add_vertex(0)
G.add_vertex(1)
G.add_vertex(2)
G.add_vertex(3)
# Agregar aristas al grafo
G.add_edge(0,1)
G.add_edge(1,2)
G.add_edge(2,3)
G.add_edge(3,0)
G.add_edge(0,2)
# Dibujar el grafo
G.show()
```

Ejemplo crear el grafo de los puentes de Königsberg
para que el grafo pueda aceptar multiples aristas en el mismo par de vertices hay que activar la opcion multi edges 
```G = Graph(multiedges=True)```
```python
# Importar la librería de grafos
G = Graph(multiedges=True)

# Agregar vértices al grafo
G.add_vertex("A")
G.add_vertex("B")
G.add_vertex("C")
G.add_vertex("D")
# Agregar aristas al grafo
G.add_edge("A","B")
G.add_edge("B","A")
G.add_edge("A","C")
G.add_edge("A","C")
G.add_edge("A","D")
G.add_edge("B","D")
G.add_edge("C","D")

# Dibujar el grafo
G.show()
```

