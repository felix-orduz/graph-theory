# Taller Grafos

### Redes Sociales
Crea un grafo que represente una red de amistades con 6 personas para alguno de los integrantes. Asegúrese de que cada persona esté conectada al menos otra personas. Representa visualmente la red social.

**Ejemplo:**
```lua
        Juan -- Maria -- Carlos
         |
       Juana -- Pedro
         |
      Camila -- Carlos
```

### Países de la OTAN y sus Fronteras
Contexto:
La Organización del Tratado del Atlántico Norte (OTAN) es una alianza militar que incluye países de América del Norte y Europa. En este ejercicio, explorarás las relaciones geopolíticas entre algunos de los países miembros de la OTAN, específicamente analizando qué países comparten fronteras terrestres. Utilizarás SageMathCell para crear un grafo en el que cada nodo representa un país de la OTAN y cada arista indica una frontera compartida.

**Instrucciones:**

- Selecciona un subconjunto de países miembros de la OTAN (minimo 7). Por ejemplo, puedes elegir Alemania, Francia, Bélgica, Países Bajos, Luxemburgo, Italia, y España.
- Crea un grafo donde cada nodo representa uno de los países seleccionados.
- Conecta los países con aristas si comparten una frontera terrestre.
- Etiqueta cada arista con el nombre de la frontera común, si es necesario.
- Visualiza el grafo para mostrar estas relaciones.

**Preguntas de análisis:**

¿Qué país tiene el mayor número de conexiones directas con otros países de la OTAN en este grafo? ¿Qué implica esto sobre su posición geopolítica dentro de Europa?
¿Cómo podrían afectar estas fronteras compartidas las políticas de defensa y las relaciones diplomáticas entre estos países?

## Ejercicio de Grafos: Análisis de Distribución de Tiendas por Localidades en Bogotá
**Contexto:**
Una cadena de tiendas tiene varias sucursales distribuidas en diferentes localidades de Bogotá, Colombia. La gerencia desea obtener una representación visual de la distribución de estas tiendas para analizar la cobertura de la cadena en la ciudad y planificar estrategias de expansión o reorganización.

**Objetivo:**
Crear un grafo en SageMathCell donde cada nodo representa una localidad de Bogotá y cada nodo está etiquetado con el número de tiendas que la cadena tiene en esa localidad. Además, se añadirán aristas entre localidades adyacentes para representar su proximidad geográfica.

Datos:
Supongamos que la cadena tiene tiendas en las siguientes localidades de Bogotá con el número de tiendas indicado:

Chapinero: 5 tiendas
Usaquén: 3 tiendas
Suba: 4 tiendas
Engativá: 2 tiendas
Teusaquillo: 3 tiendas
Kennedy: 6 tiendas
Bosa: 2 tiendas

**Instrucciones:**

Crea un grafo donde cada nodo representa una de las localidades mencionadas.
Etiqueta cada nodo con el nombre de la localidad y el número de tiendas (ejemplo: "Chapinero (5)").
Conecta los nodos con aristas si las localidades son geográficamente adyacentes. Por ejemplo, Chapinero es adyacente a Teusaquillo, Suba es adyacente a Usaquén, etc.
Visualiza el grafo para mostrar estas relaciones y etiquetas.

## Unidades de Medida en Física
**Contexto:**
En física, diferentes cantidades físicas como fuerza, masa y trabajo se miden en distintas unidades. Este ejercicio te ayudará a visualizar las relaciones entre estas unidades de medida y cómo se convierten unas en otras. Utilizando SageMathCell, crearás un grafo donde cada nodo es una unidad de medida y cada arista muestra la relación de conversión o dependencia entre las unidades.

**Unidades y sus relaciones:**

- Masa se mide en kilogramos (kg).
- Longitud se mide en metros (m).
- Tiempo se mide en segundos (s).
- Fuerza se mide en newtons (N). Un newton es equivalente a kg⋅m/s
2
kg⋅m/s 
2
 .
Energía y trabajo se miden en julios (J), donde un julio es 
N
⋅
m
N⋅m.
Instrucciones:

Crea un grafo donde cada nodo representa una unidad de medida (kg, m, s, N, J).
Conecta las unidades con aristas que representen sus relaciones, por ejemplo, cómo se calcula un newton a partir de kilogramos, metros y segundos.
Etiqueta cada arista con la relación de conversión apropiada.
Visualiza el grafo para mostrar estas relaciones.
