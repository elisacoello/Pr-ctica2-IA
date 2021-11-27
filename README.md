# Practica 2. Búsqueda heurística sin adversarios
## Elisa Coello Valverde

*Ejercicios a resolver*

**1. ¿Qué variable representa la lista ABIERTA?**
La variable que representa la lista abierta en el código es la lista openSet, donde se añade inicialmente el nudo inicial (start), esto lo podemos encontrar inicialmente en el código asi:

```

final List<Graph.Vertex> openSet = new ArrayList<Graph.Vertex>(size); // The set of tentative nodes to be evaluated, initially containing the start node openSet.add(start);
```

**2. ¿Qué variable representa la función g?**
La variable gscore es la que representa la función g en nuestro código iniciándose esta a 0 y contendrá el nudo inicial, esto lo vemos en el siguiente trozo de código:

final Map<Graph.Vertex,Integer> gScore = new HashMap<Graph.Vertex,Integer>(); // Cost from start along best known path. gScore.put(start, 0);

**3. ¿Qué variable representa la función f?**
La variable fscore es la que representa la función f, como sabemos f = g + h es una estimación positiva de ``h*(n)``, desde n hasta su objetivo, h(n) = 0 si es el objetivo. Podemos encontrar en el código f de esta forma:

final Map<Graph.Vertex,Integer> fScore = new HashMap<Graph.Vertex,Integer>();

**4. ¿Qué método habría que modificar para que la heurística representara**
**la distancia aérea entre vértices?**

**5. ¿Realiza este método reevaluación de nudos cuando se encuentra una**
**nueva ruta a un determinado vértice? Justifique la respuesta.**



https://github.com/phishman3579/java-algorithms-implementation
