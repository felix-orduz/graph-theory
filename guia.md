# Manual de Teoría de Grafos con SageMathCell y Phython

Este documento proporciona una guía paso a paso sobre cómo crear y manipular grafos utilizando SageMathCell, un recurso en línea para la computación matemática, especialmente útil para estudiantes y profesionales en el campo de la Teoría de Grafos. A continuación, se detallan los métodos para construir grafos simples, grafos con vértices nombrados individualmente y grafos con múltiples aristas entre el mismo par de vértices, como en el famoso problema de los puentes de Königsberg.


## Creación de un Grafo Simple

Acceda a [https://sagecell.sagemath.org/](https://sagecell.sagemath.org/) y en el cuadro de texto que indica **"Type some Sage code below and press Evaluate."**, puede introducir el código que se muestra a continuación.

La siguiente secuencia de comandos ilustra cómo crear un grafo básico con cuatro vértices y varias aristas. Este ejemplo es ideal para quienes se inician en la manipulación de grafos con SageMathCell:


![Ejemplo](https://i.imgur.com/RRNdu8s.png)

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
[Ver Ejemplo](https://sagecell.sagemath.org/?z=eJxljEEKwkAMRfeF3uFDN1MYpNq1C0EonkFEUieOI5WWTK1ncuEpejEbiiC6epD89zLsbl0rPQkaQhNqYRlfBMfwQuc2pkmFNSqh7mLyNEmTDBsv7CdhGJ_ShxNHUDOvp_GCnDsOPD_MvrBYWqwsysOPTRJiT_8uO6-iUTO3MKortaEsLQplofdPdBvq-3WK8lcsXtqHyd93XEA4&lang=sage&interacts=eJyLjgUAARUAuQ==)



## Crear un Grafo Nombrando Cada Vértice Individualmente

Para un control más detallado sobre la adición de vértices y aristas, puede optar por nombrar cada elemento uno por uno, como se muestra a continuación:

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
[Ver Ejemplo](https://sagecell.sagemath.org/?z=eJxljUEKgzAQRfeCdxhwk0AoGtddFAriKcrYTGOKRZmktlfqoqfwYhW7qKbbx__vZVDfhp4DMnQInWuYeHojGALLeOl9mlSwh4pxaIVMkzTJ4GCZ7HwYpxcHdyYP2H3X83iHxpxG4kBPkcsIFDHQMSjluoDsfMB_PxlLIlc_3QIKpbdAq3ILSpXLyKGX4NE19-scpFXIt_1DyA_TPVgI&lang=sage&interacts=eJyLjgUAARUAuQ==)

## Ejemplo: Crear el Grafo de los Puentes de Königsberg

Para ilustrar cómo manejar múltiples aristas entre un par de vértices, utilizaremos el famoso problema de los puentes de Königsberg. Este ejemplo requiere activar la opción `multiedges` para permitir más de una arista entre dos vértices:
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
![Ejemplo](https://i.imgur.com/h524bsA.png)

[Ver Ejemplo ](https://sagecell.sagemath.org/?z=eJyNzk0KgzAQBeC94B0G3SiU3sCFP1C6776MzTSmKMok2l6pi57CizVBSsV00e3HvHkvhmM39GyQoUVoVc3E8wtBEEjGa6_D4AAZHBiHJunG1igSknR24pHSMAiDGHLJJG1-mp9s1IU0YLuEbXaPQpwnYkOPJMqjdEuFT6VPlaNvE7LSBv0eN8217NZvFyws5lt0l-XfWP366WH5QTe4UvV4s4NpNVQ3_T1J37IDbTk=&lang=sage&interacts=eJyLjgUAARUAuQ==)
