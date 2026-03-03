## MIT 18.05 - Class 01: Introduction, Counting, and Sets | Class 02: Probability Basics - Notes

### Probabilidad
- Es una medida matemática del grado de incertidumbre asociado a la ocurrencia de un evento, expresada como un número entre 0 (imposible) y 1 (posible) o en porcentaje (0% - 100%). Se calcula dividiendo el número de casos favorables entre el total de casos posibles.
- Formalmente, la probabilidad no mide “certeza”, sino la plausibilidad de que ocurra un evento dentro de un experimento aleatorio.
- En espacios muestrales finitos y equiprobables puede calcularse con la Fórmula Laplace: Probabilidad = número de casos faborables / número de casos posibles

### Probabilidad vs. Estadística
- Probabilidad:
  - Lógicamente autónomo
  - Algunas reglas para calcular probabilidad
  - Una respuesta correcta
- Estadística:
  - Más complejo y más artístico
  - Intenta hacer inferencias basadas en probabilidad a partir de datos experimentales
  - No hay una única respuesta correcta

### Conceptos básicos
- Experimento: un procedimiento repetible
- Espacio Muestral (Sample Space) $S$: conjunto de todos los resultados posibles
- Evento: un subconjunto del espacio muestral 
- Medida de Probabilidad $P$: es una función definida sobre los eventos (subconjuntos del espacio muestral $S$) que satisface los axiomas de Kolmogorov.
  - Asigna a cada evento un número real entre 0 y 1.
  - Cumple las propiedades fundamentales de no negatividad, normalización y aditividad.

### Axiomas de Kolmorov
- Son las tres reglas fundamentales que definen el comportamiento de las probabilidades. Formuladas por Andrey Kolmogorov en 1933
- Axioma 1: No Negatividad. 
  - Para cualquier evento $A$ dentro del espacio muestral $S$, la probabilidad de que ocurra $A$ es un número real no negativo. 
  - $P(A) \ge 0$ 
- Axioma 2: Normalización (Suceso Seguro). 
  - La probabilidad del espacio muestral S completo es igual a 1. 
  - $P(S) = 1$
- Axioma 3: Aditividad (Sucesos Excluyentes).
  - Si se tienen eventos $A_1$, $A_2$, ... que son mutuamente excluyentes (no pueden ocurrir al mismo tiempo), la probabilidad de que ocurra al menos uno de ellos es la suma de sus probabilidades. 
  - $P(A_1 \cup A_2 ...) = P(A_1) + P(A_2) + ... $

### Propiedades Derivadas de los Axiomas
- Suceso Imposible:
  -  La probabilidad del conjunto vacío es cero
  -  $P(\emptyset) = 0$
-  Complemento:
   -  La probabilidad de que un evento $A$ no ocurra es 1 menos la probabilidad de que ocurra
   -  $P(A^c) = 1 - P(A)$
-  Rango:
   -  La probabilidad de cualquier evento $A$ siempre estará entre 0 y 1
   -  $0 \le P(A) \le 1$
-  Monotonía:
   -  Si el evento $A$ está contenido en el evento $B$ entonces la probabilidad $P$ de $A$ no puede ser mayor que la probabilidad $P$ de $B$
   -  $A \subseteq B \implies P(A) \le P(B)$
  
### Independencia
- Se da cuando la ocurrencia de un evento $A$ no afecta la probabilidad de ocurrencia de un evento $B$
- Por definición, dos eventos $A$ y $B$ son independientes si y solo si la probabilidad de que ambos ocurran es el producto de sus probabilidades individuales
  - $P(A \cap B) = P(A) \cdot P(B)$
- Probabilidad Condicional: Si $A$ y $B$ son independientes, saber que $B$ ha ocurrido no cambia la probabilidad de $A$
  - $P(A|B) = P(A)$

### Eventos Excluyentes (Disjuntos)
- Se da cuando dos eventos no pueden suceder al mismo tiempo; la ocurrencia de uno impide la del otro
- Su fórmula fundamental es la Regla de la Adición, donde la probabilidad de que ocurra $A$ o $B$ es la suma de sus probabilidades individuales
  - $P(A \cup B) = P(A) + P(B)$
- Por definición, dos eventos son mutuamente excluyentes si no comparten resultados comunes. Entonces la probabilidad conjunta es igual a 0
  - $P(A \cap B) = 0$
- Si $P(A) > 0$ y $P(B) > 0$ entonces los eventos excluyentes no pueden ser independientes
- Ejemplo: al lanzar un dado, sacar un 2 (evento $A$) y sacar un 5 (evento $B$) son excluyentes, ya que no puede salir ambos números a la vez

### Eventos Incluyentes
- Se da cuando dos eventos pueden suceder al mismo tiempo, es decir, tienen resultados en común
- Su fórmula fundamental es la Regla General de Suma
  - Para cualesquiera dos eventos $A$ y $B$:
  - $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
  - Esta fórmula evita contar dos veces la intersección cuando los eventos no son disjuntos.
- Ejemplo: al sacar una carta de una baraja, obtener un As (evento $A$) y obtener una carta roja (evento $B$). Pueden ocurrir juntos si se saca el As de corazones o el As de diamantes. Por tanto, se deben restar las cartas que son a la vez As y rojas para no contarlas dos veces


## Observaciones Matemáticas

- La independencia es una relación multiplicativa: $P(A \cap B) = P(A) \cdot P(B)$.
- La exclusión mutua es una relación aditiva: $P(A \cap B) = 0$.
- Si $P(A) > 0$ y $P(B) > 0$, entonces eventos mutuamente excluyentes no pueden ser independientes.
- Los axiomas de Kolmogorov permiten definir la probabilidad de forma abstracta, sin depender necesariamente de la interpretación frecuentista.
    
