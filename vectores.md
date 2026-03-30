# Vectores
---
## 📌 Problemas Resueltos
### Problema 1
```{admonition} Módulo y dirección de un vector
:class: important
Se analiza el movimiento de una partícula cargada dentro de un campo magnético deflector. El acelerómetro reporta que la aceleración instantánea de la partícula cargada está definida por el vector $\vec{a} = (2.0 \hat{i} + 3.0 \hat{j}) \, \text{m/s}^2$. Como ingeniero a cargo, debes determinar la **intensidad total** (módulo) de la aceleración y el **ángulo de director** ($\theta$) respecto al eje de referencia horizontal para calibrar los imanes deflectores. Un ángulo superior a $70^\circ$ hará que la partícula se desvie mucho y no impacte en la pantalla


```{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Position_vector.svg/250px-Position_vector.svg.png
:alt: vector aceleracion
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

#### 1. Marco Teórico
* **Fenómeno:** Representación de una magnitud física vectorial mediante sus componentes rectangulares.
* **Ruta de solución:** Utilizaremos la descomposición analítica para hallar la magnitud mediante el Teorema de Pitágoras y la dirección mediante trigonometría inversa.
* **Predicción cualitativa:** Dado que la componente vertical ($3.0$) es mayor que la horizontal ($2.0$), el vector estará más inclinado hacia el eje $y$, por lo que esperamos un ángulo mayor a $45^\circ$.

#### 2. Resolución Técnica
Siguiendo los pasos analíticos para la calibración del sistema:

1. **Expresamos $\vec{A}$ en función de sus componentes:**
   $$\vec{A} = (2.0 \hat{i} + 3.0 \hat{j}) \, \text{m/s}^2$$

2. **Calculamos el módulo de $\vec{A}$:**
   $$A = \sqrt{2^2 + 3^2} = \sqrt{13} \approx 3.6055...$$
   Reportando con la precisión adecuada: **$A = 3.6 \, \text{m/s}^2$**

3. **Calculamos la dirección y sentido de $\vec{A}$:**
   $$\theta = \tan^{-1} \left( \frac{3}{2} \right)$$
   $$\theta = 56.309...^\circ \implies \mathbf{\theta = 56^\circ}$$

#### 3. Discusión Crítica
* 🔴 **Rojo:** El modelo asume un sistema de coordenadas ideal con valores exactos. En la práctica, la vibración del sensor podría introducir un "ruido" en las componentes.
* 🟢 **Verde:** El resultado $\theta = 56^\circ$ es coherente con nuestra predicción inicial (es mayor a $45^\circ$).
* 🔵 **Azul:** Una aceleración de $3.6 \, \text{m/s}^2$ es razonable para equipos de laboratorio estándar.

#### 4. Análisis de Sensibilidad ("¿Y si...?")
* Si la componente horizontal $A_x$ se reduce a la mitad ($1.0$), el ángulo aumentaría a $71.57^\circ$, haciendo que la deflexión sea mucho más vertical. La precisión en el eje $x$ es crítica para el impacto de la partícula.

#### 5. Transferencia y Extensión
* **En un acelerador de partículas, estas son desviadas por la acción de campo magnéticos y eléctricos.

✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Dibuja los siguientes vectores en tu cuaderno, luego mide el módulo y el ángulo director de cada vector. Contrasta tus medidas con los resultados análiticos o teóricos. Justifica tu respuesta basándote en las reglas de redondeo:

Campo Magnético: $\vec{B} = (-3.2 \hat{i} + 3.2 \hat{j}) \, \text{mT}$

Fuerza de Tensión: $\vec{T} = (5.0 \hat{i} - 24.0 \hat{j}) \, \text{kN}$

Momento de Fuerza de par Motor: $\vec{M} = (-12.4 \hat{i} - 8.5 \hat{j}) \, \text{kNm}$

**Reto Metacognitivo:** En el primer ejercicio ($\vec{B}$), el ángulo que arroja la calculadora es $-45^\circ$. Sin embargo, el vector está en el segundo cuadrante. ¿Cómo expresarías el ángulo director real medido desde el eje $+x$?

```
---

### Problema 2

```{admonition} Descomposición rectangular
En el diseño de un anclaje para una torre de telecomunicaciones, se identifica una fuerza de tensión $\vec{F}$ cuya magnitud es de $12.5 \, \text{N}$ y actúa con un ángulo de inclinación de $231.4^\circ$ respecto al eje de referencia $+x$. Como parte del equipo de diseño, debes expresar esta fuerza en sus **componentes rectangulares** $(\hat{i}, \hat{j})$ para determinar la carga que recibe cada eje del soporte.

```{figure} https://www.siyavula.com/read/za/physical-sciences/grade-11/vectors-in-two-dimensions/images/237558d0d2f3372af9e58f9a39d3e84e.png
:alt: vector fuerza
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

#### 1. Marco Teórico e Hipótesis Inicial
* **Fenómeno:** Descomposición de un vector en un sistema de coordenadas cartesianas mediante proyecciones trigonométricas.
* **Ruta de solución:** Aplicaremos las funciones seno y coseno para proyectar la magnitud sobre los ejes ortogonales.
* **Predicción cualitativa:** Dado que el ángulo es de $231.4^\circ$, el vector se ubica en el **tercer cuadrante**. Se espera que ambas componentes ($F_x$ y $F_y$) resulten **negativas**.

#### 2. Resolución Técnica
1. **Descomposición escalar de la fuerza:**
   - $F_x = 12.5 \, \cos(231.4^\circ) = 12.5 \, (-0.623879...) = -7.79849... \, \text{N}$
   - $F_y = 12.5 \, \sin(231.4^\circ) = 12.5 \, (-0.781520...) = -9.76900... \, \text{N}$

2. **Aplicación de Cifras Significativas (3 C.S.):**
   Basándonos en la magnitud de la fuerza ($12.5$):
   - $F_x = -7.80 \, \text{N}$
   - $F_y = -9.77 \, \text{N}$

3. **Expresión vectorial final:**
   $$\vec{F} = (-7.80 \hat{i} - 9.77 \hat{j}) \, \text{N}$$

#### 3. Discusión Crítica (Semáforo)
* 🔴 **Rojo:** Pequeños errores en la medición del ángulo podrían cambiar la distribución de carga.
* 🟢 **Verde:** La predicción se cumple; ambas componentes son negativas, confirmando la posición en el tercer cuadrante.
* 🔵 **Azul:** Los valores son menores a $12.5 \, \text{N}$, lo cual es consistente. La componente vertical es mayor a la horizontal, lo que indica una carga más pesada hacia el eje $-y$.

#### 4. Análisis de Sensibilidad ("¿Y si...?")
* Si el ángulo fuera exactamente $225^\circ$ (diagonal perfecta), las componentes serían iguales ($8.84 \, \text{N}$). Al estar en $231.4^\circ$, hemos desplazado casi $1 \, \text{N}$ de carga del eje $x$ hacia el eje $y$. En estructuras de gran escala, este "ruido" en la medición del ángulo puede determinar si un perno de anclaje falla o resiste.

#### 5. Transferencia y Extensión
Las torres de alta tensión están sujetas a tensiones mecánicas complejas debido al peso de los conductores y la acción del viento. Descomponer estas fuerzas es vital para calcular las cargas verticales (que comprimen la estructura y cimentación) y las horizontales (que generan momentos de vuelco), asegurando que los aisladores y soportes operen siempre dentro de los márgenes de seguridad técnica.

✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Dibuja en tu cuaderno, mide el módulo y el ángulo director de cada vector, contrasta tus medidas con los resultados análiticos o teóricos. Justifica tu respuesta basándote estrictamente en las reglas de redondeo y la cantidad de C.S. de los datos de entrada:

Campo Magnético: $\vec{B} = (-3.2 \hat{i} + 3.2 \hat{j}) \, \text{mT}$

Fuerza de Tensión: $\vec{F} = (5.0 \hat{i} - 24.0 \hat{j}) \, \text{kN}$

Torque de un Motor: $\vec{M} = (-12.4 \hat{i} - 8.5 \hat{j}) \, \text{kNm}$

**Reto Metacognitivo:** En el primer ejercicio ($\vec{B}$), el ángulo que arroja la calculadora es $-45^\circ$. Sin embargo, el vector está en el segundo cuadrante. ¿Cómo expresarías el ángulo director real medido desde el eje $+x$? ¿Cuántas cifras significativas debería tener tu respuesta final para ser técnicamente honesta?

```
---

### Problema 3
```{admonition} El trabajo mecánico de una fuerza
:class: important
Una cuadrilla de operarios transportan un transformador una distancia horizontal de $2.5 \, \text{m}$. La fuerza que empuja el cuerpo tiene una magnitud de $1000 \, \text{N}$ y forma un ángulo de $28^\circ$ con el vector desplazamiento. Como ingeniero, calcula el **trabajo mecánico** ($W$) realizado por la fuerza totla de los operarios para evaluar la transferencia energética del proceso.
```

```{admonition} Solución
:class: dropdown hint

#### 1. Marco Teórico e Hipótesis Inicial
* **Fenómeno:** Transferencia de energía mediante trabajo mecánico definido por el producto escalar.
* **Ruta de solución:** Utilizaremos la definición geométrica del producto escalar: $W = \vec{F} \cdot \Delta \vec{r} = |\vec{F}| |\Delta \vec{r}| \cos(\theta)$.
* **Predicción cualitativa:** Dado que el ángulo es agudo ($28^\circ < 90^\circ$), el trabajo será **positivo**, lo que significa que la fuerza está inyectando energía al sistema en la dirección del movimiento.

#### 2. Resolución Técnica
1. **Identificamos los vectores en forma de magnitud y ángulo:**
   - $|\vec{F}| = 1000 \, \text{N}$
   - $|\Delta \vec{r}| = 2.5 \, \text{m}$
   - $\theta = 28^\circ$

2. **Aplicamos el Producto Escalar:**
   $$W = (1000 \, \text{N}) \, (2.5 \, \text{m}) \, \cos(28^\circ)$$
   $$W = 2207.36... \, \text{J}$$

3. **Redondeo y Resultado Final:**
   Considerando que la medida de distancia ($2.5$) y el ángulo ($28$) limitan nuestra precisión a 2 C.S.:
   $W = 2.2 \times 10^3 \, \text{J}$ 

#### 3. Discusión Crítica (Semáforo)
* 🔴 **Rojo:** Se está ignorando la fuerza de fricción del suelo. Mayor fuerza de friccón, mayor sería la fuerza aplicada y mayor el trabajo desarrollado.
* 🟢 **Verde:** El resultado es positivo, lo cual es coherente ya que la fuerza "apoya" el desplazamiento.
* 🔵 **Azul:** Un valor de $2200 \, \text{J}$ es una cantidad de energía pequeña en términos biológicos; por ejemplo, representa apenas el $50\%$ de la energía química contenida en una galleta promedio ($4180 \, \text{J}$). Es un valor razonable para un desplazamiento manual corto.

#### 4. Análisis de Sensibilidad ("¿Y si...?")
* ¿Qué pasaría si el ángulo aumentara a $90^\circ$? El trabajo sería **cero**. Aunque se aplique fuerza, si esta es perpendicular al desplazamiento, no contribuye a la transferencia de energía en esa dirección.

#### 5. Transferencia y Extensión
* **Ingeniería Eléctrica:** En las maniobras de mantenimiento de campo, las cuadrillas eléctricas a menudo deben movilizar componentes pesados como motores de repuesto o transformadores. Utilizar herramientas con ruedas o plataformas rodantes disminuye drásticamente la fricción, permitiendo que la fuerza aplicada disminuya y se transforme en un trabajo mecánico mucho más efectivo y facilitando las maniobras seguras en los espacios reducidos de una subestación..

✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Calcula el producto escalar (Trabajo) para los siguientes casos de diseño:

$|\vec{F}| = 500 \, \text{N}; \Delta \vec{r} = 10.0 \, \text{m}; \theta = 145^\circ$

**Reto Metacognitivo:** Considerando el análisis de la maniobra de la cuadrilla eléctrica, ¿bajo qué condiciones geométricas el trabajo desarrollado por la fuerza aplicada es máximo? ¿Cómo impacta un ángulo de inclinación excesivo (cercano a $90^\circ$) en la fatiga del operario y en la eficiencia real de la tarea de mantenimiento?

```
---
### Problema 4

```{admonition} Trabajo mecánico de operarios
:class: important
Tres operarios de mantenimiento ejercen fuerzas sobre un gabinete eléctrico pesado para desplazarlo a través de un plano inclinado. Las fuerzas aplicadas son:
- $\vec{F}_1 = (400 \hat{i} + 300 \hat{j}) \, \text{N}$
- $\vec{F}_2 = (1200 \hat{i} + 500 \hat{j}) \, \text{N}$
- $\vec{F}_3 = (500 \hat{i} + 100 \hat{j}) \, \text{N}$

El desplazamiento logrado por la caja es $\Delta \vec{r} = (2.0 \hat{i} + 1.5 \hat{j}) \, \text{m}$. Determina el **trabajo total de los operarios** realizado sobre el gabinete para verificar si la maniobra cumplió con los objetivos de energía del plan de trabajo.


```{figure} https://org-dcmp-staticassets.s3.us-east-1.amazonaws.com/posterimages/1788_1.jpg
:alt: plano inclinado. (Fuente: DCMP)
:width: 400px
:align: center
```

```{admonition} Solución
:class: dropdown hint

#### 1. Marco Teórico e Hipótesis Inicial
* **Fenómeno:** Superposición de fuerzas y cálculo de trabajo mediante el producto escalar analítico.
* **Ruta de solución:** Primero se determina la fuerza neta ($\vec{F}_{neta}$) sumando vectorialmente las contribuciones individuales y luego se calcula el producto escalar con el vector desplazamiento.
* **Predicción cualitativa:** Al ser todas las componentes positivas, la fuerza resultante y el desplazamiento apuntan en la misma dirección general, por lo que el trabajo neto será **positivo**.

#### 2. Resolución Técnica
1. **Cálculo de la Fuerza Neta ($\vec{F}_{neta}$):**
   $$\vec{F}_{neta} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3$$
   $$\vec{F}_{neta} = (400+1200+500)\hat{i} + (300+500+100)\hat{j}$$
   $$\vec{F}_{neta} = (2100 \hat{i} + 900 \hat{j}) \, \text{N}$$

2. **Cálculo del Trabajo Neto ($W_{neto}$):**
   $$W_{neto} = \vec{F}_{neta} \cdot \Delta \vec{r}$$
   $$W_{neto} = (2100 \hat{i} + 900 \hat{j}) \cdot (2.0 \hat{i} + 1.5 \hat{j})$$
   $$W_{neto} = 2100(2.0) + 900(1.5) = 4200 + 1350 = 5550 \, \text{J}$$

3. **Resultado Final (Cifras Significativas):**
   Dado que el desplazamiento tiene 2 C.S. ($2.0$ y $1.5$):
   **$W_{neto} = 5.6 \times 10^3 \, \text{J}$** (Reporte de ingeniería con rigor técnico).

#### 3. Discusión Crítica (Semáforo)
* 🔴 **Rojo:** No se ha considerado la fuerza de gravedad ni la fricción del plano inclinado, que actúan en sentido opuesto al movimiento, el trabajo neto de todas fuerzas sería menor.
* 🟢 **Verde:** La fuerza neta apunta al primer cuadrante, al igual que el desplazamiento, validando el signo positivo.
* 🔵 **Azul:** $5550 \, \text{J}$ es una cantidad de energía considerable; equivale aproximadamente a la energía que consume un motor pequeño de 1 HP operando por unos 7 segundos.

#### 4. Análisis de Sensibilidad ("¿Y si...?")
* ¿Qué pasaría si el desplazamiento fuera perpendicular a la fuerza neta? El trabajo sería nulo. La eficiencia de la maniobra depende de que los técnicos coordinen sus fuerzas lo más alineadas posible al vector desplazamiento.

#### 5. Transferencia y Extensión
* **Ingeniería Eléctrica:** El movimiento de transformadores de gran escala en subestaciones requiere la acción coordinada de múltiples cabrestantes o técnicos. Comprender cómo se suman estas fuerzas permite al supervisor garantizar que la fuerza neta sea suficiente para vencer la inercia y la fricción sin comprometer la integridad de los operarios.

```
---
## 📓 Actividades para el Portafolio Digital

Como futuro ingeniero de la FIEE, tu portafolio no es solo una colección de ejercicios, sino un registro de tu juicio crítico. Desarrolla los siguientes desafíos:

**Desafío 1: El Límite de Seguridad en la Torre**

Dos fuerzas de tensión actúan sobre un aislador de una torre de transmisión: $\vec{F}_1 = (500 \hat{i} + 1200 \hat{j}) \, \text{N}$ y $\vec{F}_2 = (900 \hat{i} + 1200 \hat{j}) \, \text{N}$.

- El Conflicto: El fabricante del aislador garantiza que este solo soporta una fuerza resultante máxima de $2.5 \, \text{kN}$.

- La Tarea: Calcula el módulo de la fuerza resultante. ¿Está el sistema operando en la zona de seguridad?

- El Veredicto: Como ingeniero supervisor, ¿autorizas la operación o exiges un refuerzo inmediato? .

**Desafío 2: La Maniobra del Dron de Mantenimiento**

Un dron de inspección de líneas debe ser lanzado con una velocidad de $22.2 \, \text{m/s}$ formando un ángulo de $62^\circ$ con la horizontal para evitar una descarga de arco eléctrico.

- El Conflicto: El dron necesita una velocidad vertical mínima de $18 \, \text{m/s}$ para estabilizarse antes de llegar a los cables.

- La Tarea: Calcula las componentes horizontal y vertical de la velocidad.

**Desafío 3: El Error de Logística en la Subestación**

Un técnico realiza tres desplazamientos sucesivos para localizar una falla en una red subterránea: $\vec{\Delta r}_1 = (400 \hat{i} + 300 \hat{j}) \, \text{m}$, $\vec{\Delta r}_2 = (-1000 \hat{i} + 800 \hat{j}) \, \text{m}$ y $\vec{\Delta r}_3 = (1400 \hat{i} - 1300 \hat{j}) \, \text{m}$.

- El Conflicto: El manual dice que la falla está a no más de $500 \, \text{m}$ en línea recta desde el punto de inicio.

- La Tarea: Calcula el módulo del desplazamiento total.

- La Reflexión: ¿Qué distancia total caminó el técnico (escalar) frente a qué tan lejos está realmente del inicio (vector)? ¿Por qué en ingeniería de mantenimiento "distancia" y "desplazamiento" pueden significar la diferencia entre encontrar una falla o perderse en el campo?

**Desafío 4: Eficiencia en el Plano Inclinado**

Se debe subir un transformador sobre un plano inclinado de $30^\circ$. Se aplica una fuerza de $500 \, \text{N}$ con un ángulo de $43^\circ$ respecto a la horizontal.

- El Conflicto: El operario cree que mientras más "hacia arriba" empuje, más fácil será el trabajo. Sin embargo, el ángulo real entre la fuerza y el camino (el plano) es lo que cuenta.

- La Tarea: Calcula el trabajo realizado. (Cuidado: Identifica correctamente el ángulo entre el vector fuerza y el vector desplazamiento).

- El Reto: ¿Bajo qué ángulo el trabajo desarrollado sería máximo? ¿Qué le recomendarías al operario para no desperdiciar energía?

**Desafío 5: Mesa de Fuerzas y Equilibrio Real**

- Desarrolla el experimento de la Mesa de Fuerzas y documenta lo siguiente en tu Diario de Aprendizaje:

- Conflicto Experimental: Al colocar las pesas en proporción 3, 4 y 5, ¿lograste el equilibrio perfecto a la primera?

- Evidencia: Inserta fotos donde se vea el anillo centrado y los ángulos medidos con el transportador.

- Tarea Crítica: Comprueba mediante el método de componentes si la suma vectorial de tus pesas reales da exactamente cero. Si no es así, ¿a qué le atribuyes la diferencia (fricción de las poleas, error de la balanza, etc.)?

- Mira algunos videos para ayudarte en el diseño y construcción de tu mesa de fuerzas:  

    - [Video 1](https://youtube.com/shorts/OuNLTRZL7ME?si=SjT5gfrGv1KCkZZs)
    - [Video 2](https://youtu.be/0TyVb26JNJk?si=7kiCcd18D6_5FYDj)
    - [Video 3](https://www.youtube.com/watch?v=NLVCpWGOWTs)

---
## 🎯 [¡Autoevaluate!](https://gemini.google.com/share/a2c7b6dcdbea)