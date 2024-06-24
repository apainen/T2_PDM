# T2_PDM

**Rodolfo Cruz y Antonia Painen**

## Desarrollo de la tarea, archivo **Tarea2_PDM.ipynb**
Fue desarrollado en Colab, esta distribuido principalmente en tres partes deacuerdo a la estructura del enunciado. Además cada uno de esos puntos se relaciona con otros de la seccion **Problemas a Resolver** del enunciado.

En el video hacemos referencia a supuestos que hicimos, siempre teniendo en cuenta lo que especificaba en el enunciado, que en ciertas partes era ambiguo.

### **1.1. Precalentamiento: triángulos**
1. Implementa una función que reciba un grafo en Neo4j y genere una RDD con las aristas de ese grafo.
2. Implementa un programa en PySpark que entregue todos los triángulos (como tuplas de tres nodos)

### **1.2. Precalentamiento2: triángulos que usen cualquier arista**
1. De manera similar a la parte **1.1** pero se buscan patrones de triangulos, sin importar la etiqueta.

### **3. Busqueda de patrones de 4 variables**
1. Se asume que se recibe la matriz M.
Para el desarrollo de esta parte, definimos el algoritmo basado en que la matriz M, de tamaño |A| x |L| x |A| esta compuesta con:<br>
**A**: con elementos del tipo numerico, correspondientes a variables de los nodos.<br>
**L**: con elementos del tipo numerico, correspondientes a variables de las etiquetas<br>
Mientras que la consulta, un patron con unicamente variables. Por ejemplo: **[('x', 'u', 'y'), ('y', 'u', 'z'), ('z', 'u', 'w'), ('w', 'u', 'x')]**

2. Dado un patron que tiene solo variables, y exactamentecuatro variables, entregue todos los matches de ese patrón (como tuplas de 4 nodos) b^(4)
reducers, donde b es un parámetro.
