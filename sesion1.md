# Sesión 1. Cantidades Físicas
---
## 1.1. Redondeos
Existen dos reglas principales para redondear un resultado, dependiendo del tipo de operación que estés realizando. ¡Es crucial no confundirlas!

```{admonition} 1. Para Suma y resta
:class: important
El resultado se redondea a la misma posición decimal que la medida con la menor cantidad de posiciones decimales.


**Ejemplo:**

$5.45 g + 12.1 g = 17.55 g$

El resultado de la suma es 17.55 g. Como la medida menos precisa tiene solo un decimal (12.1 g), nuestro resultado debe redondearse a un solo decimal.

Resultado final: $17.6 g$
```

```{admonition} 2. Para Multiplicación y División:
:class: important
El resultado se redondea al mismo número de cifras significativas que la medida con la menor cantidad de cifras significativas.

**Ejemplo:**

$ 12.5 m  \times  4.2 m  = 52.5 m^2$

El resultado de la suma es $52.5 m^2$. La medida menos precisa tiene dos cifras significativas (4.2 m), por lo que nuestro resultado debe redondearse a dos cifras significativas.

Resultado final: $53 m^2$
```
---

## 1.2. Vectores

### 1. ¿Qué es un Vector? (Interpretación Física)

Un **vector** $\vec{A}$ es una herramienta matemática que representa una cantidad física que requiere de dirección y sentido para exresarse integramente, los vectores tienen las siguientes características:

* **Módulo (Magnitud):** La intensidad del vector, denotada como $A$ o $|\vec{A}|$.
* **Dirección:** La orientación respecto a un sistema de referencia.
* **Sentido:** Indicado por la punta de la flecha.

La **dirección y sentido de un vector** se expresa mediante **angulos directores** con respecto a un sistema de referencia.
### 2. Componentes Rectangulares y Vectores Unitarios

Para facilitar el cálculo analítico, descomponemos un vector en sus proyecciones ortogonales utilizando los vectores unitarios $\hat{i}$ y $\hat{j}$ en el plano cartesiano:

$$\vec{A} = A_x\hat{i} + A_y\hat{j}$$

Donde las componentes se calculan como:
* $A_x = A \cos(\theta)$
* $A_y = A \sin(\theta)$
* $|\vec{A}| = \sqrt{A_x^2 + A_y^2}$

## 3. Operaciones Claves

- **Suma:** $\sum \vec{F} = (F_{1x} + F_{2x})\hat{i} + (F_{1y} + F_{2y})\hat{j}$ 

- **Producto Escalar:**  $\vec{A} \cdot \vec{B} = |\vec{A}||\vec{B}| \cos(\theta)$

- **Producto Vectorial:** $\vec{A} \times \vec{B} = (AB \sin(\theta)) \hat{n}$
---

## 📌 Problemas Resueltos

### 🧩 Problema 1:  Volumen total de un refrigerante

```{admonition}  El volumen total
:class: important
Imagina que necesitas calcular el volumen total de un refrigerante para un transformador, el refrigerante ha sido depositado en dos recipientes con precisiones distinta, tal como se muestra en la figura. Un colaborador registra los valores probables de las medidas:

$V_1 = 375 \, \text{ml}$  
$V_2 = 750 \, \text{ml}$

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/vasosgraduados.png
:alt: vasos graduados
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint
**1. Marco Teórico e Hipótesis Inicial**
* **Temática:** Adición de cantidades físicas y propagación de incertidumbre por posición decimal.
* **Ruta de la solución:** Aplicar la regla de suma/resta: el resultado se limita por la medida con la posición decimal menos precisa (mayor incertidumbre absoluta).
* **Predicción cualitativa:** El resultado final no puede ser más preciso que el dato de $750 \, \text{ml}$, donde el cero no es significativo.

**2. Resolución Técnica**
* Expresamos en notación científica para visualizar la precisión real:
    $$V_1 = 3.75 \times 10^2 \, \text{ml}$$
    $$V_2 = 7.5 \times 10^2 \, \text{ml}$$
* Suma aritmética: $(3.75 + 7.5) \times 10^2 = 11.25 \times 10^2 \, \text{ml}$.
* **Redondeo Crítico:** Como $7.5 \times 10^2$ tiene solo un decimal en su mantisa, el resultado debe redondearse a un decimal.
    **Resultado Final:** $11.3 \times 10^2 \, \text{ml}$ (equivalente a $1130 \, \text{ml}$).

**3. Discusión Crítica (Semáforo de Ingeniería)**
* 🔴 **Rojo (Limitaciones):** Se asume que el cero en $750$ es un marcador de posición y no una cifra medida. Si el instrumento garantizara exactitud en las unidades, el cálculo cambiaría.
* 🟢 **Verde (Validación):** El resultado $1130 \, \text{ml}$ refleja la realidad de la medición; la "incertidumbre" del segundo frasco domina el resultado.
* 🔵 **Azul (Interpretación):** En el llenado de aceites dieléctricos, ignorar esta regla podría causar una lectura falsa de los niveles de seguridad en el tanque.

**4. Análisis de Sensibilidad ("¿Y si...?")**
¿Qué pasaría si el segundo recipiente fuera digital y marcara $750.0 \, \text{ml}$? En ese caso, la medida tendría 4 C.S., y el resultado final sería exactamente $1125 \, \text{ml}$, ya que la precisión permitiría validar las unidades.

**5. Transferencia y Extensión**
Este criterio es vital al calcular la masa total de una estructura de soporte (torres de alta tensión) donde se suman pesos de componentes medidos con distintas básculas.

✍️ **Hazlo Tú: Desafío de Precisión**

Identifica que resultados son coreccto o incorrectos, justifica tu respuesta.

- Suma de volúmenes: $3.21 \text{ dl} + 4.321 \text{ dl} = 7.53 \text{ dl}$

- Diferencia de masas: $8.25 \text{ g} - 1.2 \text{ g} = 7.05 \text{ g}$

- Carga en líneas de alta tensión: $8200 \text{ kN} - 245 \text{ kN} = 8.0 \times 10^3 \text{ kN}$
(Pista: Expresa 8200 en notación científica asumiendo que los ceros no son significativos).

- Intervalo de tiempo en osciloscopio: $0.846 \text{ s} + 0.345 \text{ s} = 1.191 \text{ s}$

```
---

### 🧩 Problema 2:  Resistencia Eléctrica

```{admonition}  La Resistencia Eléctrica
:class: important

Para obtener la resistencia eléctrica de un componente se mide la diferencia de potencial o voltaje ($V$) y la intensidad de corriente eléctrica ($I$). 
En la figura se muestra la lectura de los instrumentos:

- $V = 1.35 \, \text{V}$
- $I = 2.9 \, \text{A}$

¿Cuánto es el valor de la resistencia eléctrica $R = V/I$?

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/leydeohm.jpg
:alt: ley de ohm
:width: 60%
:align: center
```

```{admonition} Solución
:class: dropdown hint
**1. Marco Teórico e Hipótesis Inicial**
* **Temática:** Cifras Significativas (C.S.) en multiplicación y división.
* **Ruta de la solución:** Aplicar la Ley de Ohm ($R = V/I$). El resultado debe tener el mismo número de C.S. que la cantidad con menos cifras de los datos originales.
* **Predicción cualitativa:** La corriente ($2.9 \, \text{A}$) limitará el resultado a solo 2 cifras significativas.

**2. Resolución Técnica**
* Cálculo nominal: $R = \frac{1.35 \, \text{V}}{2.9 \, \text{A}} = 0.46551724... \, \Omega$
* Aplicando regla de C.S. (Redondeo a 2 cifras):
    **Resultado Final:** $0.47 \, \Omega$

**3. Discusión Crítica (Semáforo de Ingeniería)**
* 🔴 **Rojo (Limitaciones):** No se considera la resistencia interna de los cables del multímetro, que en valores menores a $1 \, \Omega$ suele ser significativa.
* 🟢 **Verde (Validación):** Reportar $0.47 \, \Omega$ es científicamente honesto. Poner más decimales sería "inventar" precisión que el amperímetro no proporcionó.
* 🔵 **Azul (Interpretación):** Este valor sugiere un componente de alta conducción o un bobinado de motor de gran calibre.

**4. Análisis de Sensibilidad ("¿Y si...?")**
Si sustituimos el amperímetro analógico por uno de precisión que marque $2.900 \, \text{A}$ (4 C.S.), la limitación pasaría al voltímetro ($1.35 \, \text{V}$), y el resultado sería $0.466 \, \Omega$.

**5. Transferencia y Extensión**
En el diseño de Shunts para medición de corriente, la precisión del valor de resistencia determina el error de toda la medición del sistema de potencia.

✍️ **Hazlo Tú: Desafío de Precisión**

Identifica que resultados son coreccto o incorrectos, justifica tu respuesta.

- Rapidez de un móvil = $v = 425 \, \text{m} / 12 \, \text{s} = 35 \, \text{m/s}$ 
- Aceleración de un camión: $a = 22.35 \, \text{m/s} / 1.02 \, \text{s} = 21.9117647 \, \text{m/s}^2$
- Densidad de un material: $\rho = 254.3 \, \text{g} / 25.3 \, \text{cm}^3 = 10.1 \, \text{g/cm}^3$$
- Torque de una fuerza:  $\tau = 124.32 \, \text{mN} \cdot 0.3 \, \text{m} = 37.296 \, \text{mN} \cdot \text{m}$

💡 **Reflexión para el Estudiante**

Nota la diferencia: En el calculo del torque de una fuerza, aunque la fuerza se midió con muchísima precisión ($124.32$), la incertidumbre en la distancia ($0.3$) "arruinó" la precisión del resultado final. En ingeniería, tu resultado es tan confiable como tu medida más descuidada.
```
---

### 🧩 Problema 3:  Área de una pila

```{admonition}  Área circular
:class: important
Se mide el diámetro de una pila con un vernier, obteniendo $d = 19.95 \, \text{mm}$. Queremos hallar el área superficial ($A = \pi d^2 / 4$). 
**Pregunta de reflexión:** Si $\pi$ tiene infinitos decimales en la memoria de la calculadora, ¿cuántos de ellos "hereda" mi resultado final?

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/vernierdiametro.jpg
:alt: diametro con vernier
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Marco Teórico e Hipótesis Inicial**
* **Temática:** Manejo de constantes exactas ($\pi$, $4$) en el cálculo de áreas.
* **Ruta de la solución:** Las constantes no limitan la precisión. El número de C.S. del resultado final dependerá exclusivamente de la medida del diámetro.
* **Predicción cualitativa:** El resultado debe mantener 4 C.S.

**2. Resolución Técnica**
* Cálculo con alta precisión para $\pi$: $A = \frac{\pi \cdot (19.95 \, \text{mm})^2}{4} = 312.5904325... \, \text{mm}^2$
* Ajuste a 4 C.S. (basado en $19.95$):
    **Resultado Final:** $312.6 \, \text{mm}^2$

**3. Discusión Crítica (Semáforo de Ingeniería)**
* 🔴 **Rojo (Limitaciones):** Se asume una sección circular perfecta. El desgaste del conductor o la presión del vernier podrían alterar la lectura real.
* 🟢 **Verde (Validación):** El redondeo hacia arriba ($0.59 \to 0.6$) es correcto según las normas de la IEEE para reporte de datos.
* 🔵 **Azul (Interpretación):** Un área de $312.6 \, \text{mm}^2$ es fundamental para determinar la dimensión donde se alojara la pila.

**4. Análisis de Sensibilidad ("¿Y si...?")**
Si el diámetro se midiera con una regla común como $20 \, \text{mm}$ (1 o 2 C.S.), el área calculada sería $3 \times 10^2 \, \text{mm}^2$, perdiendo toda la información crítica para el diseño de ingeniería.

**5. Transferencia y Extensión**
Las dimensiones de los dispositivos modernos están estrictamente sujetas a la precisión de sus componentes internos. 
* **Caso de estudio:** Piensa en el alojamiento de una batería en un celular. El espacio debe diseñarse considerando no solo el valor nominal ($312.6 \, \text{mm}^2$ de sección), sino también la **tolerancia**. 
* Si el ingeniero de diseño redondea mal o ignora la incertidumbre, la batería podría no encajar en el chasis de aluminio o, peor aún, quedar con juego interno, provocando que los pines de conexión se rompan con el uso diario. ¡La física de primer ciclo define la vida útil de tu smartphone!

✍️  **Hazlo Tú: Calculos con Fórmulas Físicas**
Identifica que resultados son coreccto o incorrectos, justifica tu respuesta.
- Volumen  = V = $(1.23 \, cm)(1.7 \, cm)(2.345 \, cm)$ = 4.9 \, \text{cm}^3$
- Velocidad = V = $(1.25 \, m/s^2)(24.56 \, s)$ = $31 \, \text{m/s}$ 
- Altura = H = $(0.5)(9.81 \, m/s^2)(1.255 \, s)^2$ =  $7.73 \, \text{m}$
- Altura = H = $(0.5)(9.8 \, m/s^2)(1.255 \, s)^2$ = $7.7 \, \text{m}$

💡 **Conclusión**
Nota la diferencia entre los ejercicios 3 y 4. Un cambio en la precisión de la constante de gravedad ($9.81$ vs $9.8$) cambió totalmente la validez de tu resultado. Como ingeniero, siempre debes elegir constantes que tengan, al menos, la misma cantidad de cifras significativas que tus mediciones de campo.

```

### 🧩 Problema 4: Haz en Campo Magnético
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

**1. Marco Teórico**
* **Fenómeno:** Representación de una magnitud física vectorial mediante sus componentes rectangulares.
* **Ruta de solución:** Utilizaremos la descomposición analítica para hallar la magnitud mediante el Teorema de Pitágoras y la dirección mediante trigonometría inversa.
* **Predicción cualitativa:** Dado que la componente vertical ($3.0$) es mayor que la horizontal ($2.0$), el vector estará más inclinado hacia el eje $y$, por lo que esperamos un ángulo mayor a $45^\circ$.

**2. Resolución Técnica**
Siguiendo los pasos analíticos para la calibración del sistema:

1. **Expresamos $\vec{A}$ en función de sus componentes:**
   $$\vec{A} = (2.0 \hat{i} + 3.0 \hat{j}) \, \text{m/s}^2$$

2. **Calculamos el módulo de $\vec{A}$:**
   $$A = \sqrt{2^2 + 3^2} = \sqrt{13} \approx 3.6055...$$
   Reportando con la precisión adecuada: **$A = 3.6 \, \text{m/s}^2$**

3. **Calculamos la dirección y sentido de $\vec{A}$:**
   $$\theta = \tan^{-1} \left( \frac{3}{2} \right)$$
   $$\theta = 56.309...^\circ \implies \mathbf{\theta = 56^\circ}$$

**3. Discusión Crítica**
* 🔴 **Rojo:** El modelo asume un sistema de coordenadas ideal con valores exactos. En la práctica, la vibración del sensor podría introducir un "ruido" en las componentes.
* 🟢 **Verde:** El resultado $\theta = 56^\circ$ es coherente con nuestra predicción inicial (es mayor a $45^\circ$).
* 🔵 **Azul:** Una aceleración de $3.6 \, \text{m/s}^2$ es razonable para equipos de laboratorio estándar.

**4. Análisis de Sensibilidad ("¿Y si...?")**
* Si la componente horizontal $A_x$ se reduce a la mitad ($1.0$), el ángulo aumentaría a $71.57^\circ$, haciendo que la deflexión sea mucho más vertical. La precisión en el eje $x$ es crítica para el impacto de la partícula.

**5. Transferencia y Extensión**
Este cálculo es fundamental en el diseño de **osciloscopios analógicos** y aceleradores lineales, donde el control vectorial de la aceleración garantiza que el haz de electrones llegue al punto exacto de la pantalla o sensor.

✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Dibuja los siguientes vectores en tu cuaderno, luego mide el módulo y el ángulo director de cada vector. Contrasta tus medidas con los resultados análiticos o teóricos. Justifica tu respuesta basándote en las reglas de redondeo:

Campo Magnético: $\vec{B} = (-3.2 \hat{i} + 3.2 \hat{j}) \, \text{mT}$

Fuerza de Tensión: $\vec{T} = (5.0 \hat{i} - 24.0 \hat{j}) \, \text{kN}$

Momento de Fuerza de par Motor: $\vec{M} = (-12.4 \hat{i} - 8.5 \hat{j}) \, \text{kNm}$

**Reto Metacognitivo:** En el primer ejercicio ($\vec{B}$), el ángulo que arroja la calculadora es $-45^\circ$. Sin embargo, el vector está en el segundo cuadrante. ¿Cómo expresarías el ángulo director real medido desde el eje $+x$?

```
---

### 🧩 Problema 5: Anclaje de Torres de Telecomunicaciones

```{admonition} Descomposición rectangular
En el diseño de un anclaje para una torre de telecomunicaciones, se identifica una fuerza de tensión $\vec{F}$ cuya magnitud es de $12.5 \, \text{N}$ y actúa con un ángulo de inclinación de $231.4^\circ$ respecto al eje de referencia $+x$. Como parte del equipo de diseño, debes expresar esta fuerza en sus **componentes rectangulares** $(\hat{i}, \hat{j})$ para determinar la carga que recibe cada eje del soporte.

```{figure} https://www.siyavula.com/read/za/physical-sciences/grade-11/vectors-in-two-dimensions/images/237558d0d2f3372af9e58f9a39d3e84e.png
:alt: vector fuerza
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Marco Teórico e Hipótesis Inicial**
* **Fenómeno:** Descomposición de un vector en un sistema de coordenadas cartesianas mediante proyecciones trigonométricas.
* **Ruta de solución:** Aplicaremos las funciones seno y coseno para proyectar la magnitud sobre los ejes ortogonales.
* **Predicción cualitativa:** Dado que el ángulo es de $231.4^\circ$, el vector se ubica en el **tercer cuadrante**. Se espera que ambas componentes ($F_x$ y $F_y$) resulten **negativas**.

**2. Resolución Técnica**
1. **Descomposición escalar de la fuerza:**
   - $F_x = 12.5 \, \cos(231.4^\circ) = 12.5 \, (-0.623879...) = -7.79849... \, \text{N}$
   - $F_y = 12.5 \, \sin(231.4^\circ) = 12.5 \, (-0.781520...) = -9.76900... \, \text{N}$

2. **Aplicación de Cifras Significativas (3 C.S.):**
   Basándonos en la magnitud de la fuerza ($12.5$):
   - $F_x = -7.80 \, \text{N}$
   - $F_y = -9.77 \, \text{N}$

3. **Expresión vectorial final:**
   $$\vec{F} = (-7.80 \hat{i} - 9.77 \hat{j}) \, \text{N}$$

**3. Discusión Crítica (Semáforo)**
* 🔴 **Rojo:** Pequeños errores en la medición del ángulo podrían cambiar la distribución de carga.
* 🟢 **Verde:** La predicción se cumple; ambas componentes son negativas, confirmando la posición en el tercer cuadrante.
* 🔵 **Azul:** Los valores son menores a $12.5 \, \text{N}$, lo cual es consistente. La componente vertical es mayor a la horizontal, lo que indica una carga más pesada hacia el eje $-y$.

**4. Análisis de Sensibilidad ("¿Y si...?")**
* Si el ángulo fuera exactamente $225^\circ$ (diagonal perfecta), las componentes serían iguales ($8.84 \, \text{N}$). Al estar en $231.4^\circ$, hemos desplazado casi $1 \, \text{N}$ de carga del eje $x$ hacia el eje $y$. En estructuras de gran escala, este "ruido" en la medición del ángulo puede determinar si un perno de anclaje falla o resiste.

**5. Transferencia y Extensión**
Las torres de alta tensión están sujetas a tensiones mecánicas complejas debido al peso de los conductores y la acción del viento. Descomponer estas fuerzas es vital para calcular las cargas verticales (que comprimen la estructura y cimentación) y las horizontales (que generan momentos de vuelco), asegurando que los aisladores y soportes operen siempre dentro de los márgenes de seguridad técnica.

✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Dibuja en tu cuaderno, mide el módulo y el ángulo director de cada vector, contrasta tus medidas con los resultados análiticos o teóricos. Justifica tu respuesta basándote estrictamente en las reglas de redondeo y la cantidad de C.S. de los datos de entrada:

Campo Magnético: $\vec{B} = (-3.2 \hat{i} + 3.2 \hat{j}) \, \text{mT}$

Fuerza de Tensión: $\vec{F} = (5.0 \hat{i} - 24.0 \hat{j}) \, \text{kN}$

Torque de un Motor: $\vec{M} = (-12.4 \hat{i} - 8.5 \hat{j}) \, \text{kNm}$

**Reto Metacognitivo:** En el primer ejercicio ($\vec{B}$), el ángulo que arroja la calculadora es $-45^\circ$. Sin embargo, el vector está en el segundo cuadrante. ¿Cómo expresarías el ángulo director real medido desde el eje $+x$? ¿Cuántas cifras significativas debería tener tu respuesta final para ser técnicamente honesta?

```
---

### 🧩 Problema 6: Trabajo Mecánico de Cuadrillas
```{admonition} El trabajo mecánico de una fuerza
:class: important
Una cuadrilla de operarios transportan un transformador una distancia horizontal de $2.5 \, \text{m}$. La fuerza que empuja el cuerpo tiene una magnitud de $1000 \, \text{N}$ y forma un ángulo de $28^\circ$ con el vector desplazamiento. Como ingeniero, calcula el **trabajo mecánico** ($W$) realizado por la fuerza totla de los operarios para evaluar la transferencia energética del proceso.
```

```{admonition} Solución
:class: dropdown hint

**1. Marco Teórico e Hipótesis Inicial**
* **Fenómeno:** Transferencia de energía mediante trabajo mecánico definido por el producto escalar.
* **Ruta de solución:** Utilizaremos la definición geométrica del producto escalar: $W = \vec{F} \cdot \Delta \vec{r} = |\vec{F}| |\Delta \vec{r}| \cos(\theta)$.
* **Predicción cualitativa:** Dado que el ángulo es agudo ($28^\circ < 90^\circ$), el trabajo será **positivo**, lo que significa que la fuerza está inyectando energía al sistema en la dirección del movimiento.

**2. Resolución Técnica**
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

**3. Discusión Crítica (Semáforo)**
* 🔴 **Rojo:** Se está ignorando la fuerza de fricción del suelo. Mayor fuerza de friccón, mayor sería la fuerza aplicada y mayor el trabajo desarrollado.
* 🟢 **Verde:** El resultado es positivo, lo cual es coherente ya que la fuerza "apoya" el desplazamiento.
* 🔵 **Azul:** Un valor de $2200 \, \text{J}$ es una cantidad de energía pequeña en términos biológicos; por ejemplo, representa apenas el $50\%$ de la energía química contenida en una galleta promedio ($4180 \, \text{J}$). Es un valor razonable para un desplazamiento manual corto.

**4. Análisis de Sensibilidad ("¿Y si...?")**
* ¿Qué pasaría si el ángulo aumentara a $90^\circ$? El trabajo sería **cero**. Aunque se aplique fuerza, si esta es perpendicular al desplazamiento, no contribuye a la transferencia de energía en esa dirección.

**5. Transferencia y Extensión**
* **Ingeniería Eléctrica:** En las maniobras de mantenimiento de campo, las cuadrillas eléctricas a menudo deben movilizar componentes pesados como motores de repuesto o transformadores. Utilizar herramientas con ruedas o plataformas rodantes disminuye drásticamente la fricción, permitiendo que la fuerza aplicada disminuya y se transforme en un trabajo mecánico mucho más efectivo y facilitando las maniobras seguras en los espacios reducidos de una subestación..


✍️ **Hazlo Tú: Desafío de Módulos y Direcciones**

Calcula el producto escalar (Trabajo) para los siguientes casos de diseño:

$|\vec{F}| = 500 \, \text{N}; \Delta \vec{r} = 10.0 \, \text{m}; \theta = 145^\circ$

**Reto Metacognitivo:** Considerando el análisis de la maniobra de la cuadrilla eléctrica, ¿bajo qué condiciones geométricas el trabajo desarrollado por la fuerza aplicada es máximo? ¿Cómo impacta un ángulo de inclinación excesivo (cercano a $90^\circ$) en la fatiga del operario y en la eficiencia real de la tarea de mantenimiento?

```
---
### 🧩 Problema 7: Trabajo Neto de Operarios

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

**1. Marco Teórico e Hipótesis Inicial**
* **Fenómeno:** Superposición de fuerzas y cálculo de trabajo mediante el producto escalar analítico.
* **Ruta de solución:** Primero se determina la fuerza neta ($\vec{F}_{neta}$) sumando vectorialmente las contribuciones individuales y luego se calcula el producto escalar con el vector desplazamiento.
* **Predicción cualitativa:** Al ser todas las componentes positivas, la fuerza resultante y el desplazamiento apuntan en la misma dirección general, por lo que el trabajo neto será **positivo**.

**2. Resolución Técnica**
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

**3. Discusión Crítica (Semáforo)**
* 🔴 **Rojo:** No se ha considerado la fuerza de gravedad ni la fricción del plano inclinado, que actúan en sentido opuesto al movimiento, el trabajo neto de todas fuerzas sería menor.
* 🟢 **Verde:** La fuerza neta apunta al primer cuadrante, al igual que el desplazamiento, validando el signo positivo.
* 🔵 **Azul:** $5550 \, \text{J}$ es una cantidad de energía considerable; equivale aproximadamente a la energía que consume un motor pequeño de 1 HP operando por unos 7 segundos.

**4. Análisis de Sensibilidad ("¿Y si...?")**
* ¿Qué pasaría si el desplazamiento fuera perpendicular a la fuerza neta? El trabajo sería nulo. La eficiencia de la maniobra depende de que los técnicos coordinen sus fuerzas lo más alineadas posible al vector desplazamiento.

**5. Transferencia y Extensión**

* **Ingeniería Eléctrica:** El movimiento de transformadores de gran escala en subestaciones requiere la acción coordinada de múltiples cabrestantes o técnicos. Comprender cómo se suman estas fuerzas permite al supervisor garantizar que la fuerza neta sea suficiente para vencer la inercia y la fricción sin comprometer la integridad de los operarios.

```
---

## 📓 Actividades para el Portafolio Digital

Como futuro ingeniero de la FIEE, tu portafolio no es solo una colección de ejercicios, sino un registro de tu juicio crítico. Desarrolla los siguientes desafíos:

**Desafío 1: El Dilema del Gran Premio (Análisis Crítico)**

Calcula la rapidez de un corredor que recorre $100.00 \, \text{m}$ en $9.58 \, \text{s}$.

- Aplica las reglas estrictas de cifras significativas.

- Conflicto: Si un segundo corredor hace $9.59 \, \text{s}$, ¿el redondeo oculta quién ganó?

- Tarea: Escribe un párrafo justificando en qué casos un ingeniero debe ignorar las reglas de redondeo para no perder información vital (ejemplo: cronometraje deportivo o microchips).


```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/usainbolt.jpg 
:alt: carrera de Usain Bolt
:width: 50%
:align: center
```
<!--/figuras/usainbolt.jpg  -->


**Desafío 2: La "Contaminación" de Constantes**

Repite el cálculo del área de la pila ($d = 19.95 \, \text{mm}$) pero usando solo $\pi = 3.14$.

- Compara el resultado con el obtenido usando el $\pi$ de la calculadora.

- Reflexión: ¿Cómo afectó el uso de una constante con pocas cifras significativas a tu resultado final? ¿Por qué decimos que una constante mal elegida "contamina" la precisión de una buena medición?


**Desafío 3: Aplicación Industrial: Diferencia de Presiones**

Un ingeniero debe calcular la caída de presión en una tubería comparando la lectura de los manometros mostrados en la figura. Realiza este ejercicio tanto en bar como en psi.

```{figure}  https://github.com/jnolorbe/fisica1/blob/main/figuras/manometros.jpg
:alt: manometros
:width: 80%
:align: center
```

<!--/figuras/manometros.jpg -->

**Desafío 4: El Espesor de la Incertidumbre (Experimental)**

- Mide con una regla escolar el espesor de un mazo de 100 hojas de papel.

- Calcula el espesor de una sola hoja dividiendo entre 100.

- Pregunta: ¿Cuántas cifras significativas tiene tu resultado final? ¿Por qué es más preciso medir 100 hojas que intentar medir una sola directamente con la misma regla?


**Desafió 5: El Misterio de $\pi$ (Tapas Circulares)**

- Busca dos tapas circulares de diferentes tamaños. Mide el perímetro ($P$) y el diámetro ($D$) con una cuerda y regla.

- Calcula $P/D$.

- Pregunta: ¿Tus resultados son idénticos para ambas tapas? ¿Cuántas cifras significativas puedes garantizar honestamente?

**Desafió 6: El Espesor de la Incertidumbre (100 Hojas)**

- Mide con una regla el espesor de un mazo de 100 hojas de tu cuaderno.

- Divide entre 100 para hallar el espesor de una hoja.

- Reflexión: ¿Por qué es físicamente más preciso medir un bloque de 100 hojas que intentar medir una sola directamente?

**Desafío 7. Presupuesto de Ingeniería (Tu Habitación)**

- Mide las dimensiones de tu piso y busca un cerámico en una tienda online.

- Calcula las cajas necesarias (incluye 5% de desperdicio).

- Decisión Técnica: ¿Redondearías la cantidad de cajas hacia abajo por matemática o hacia arriba por seguridad de obra? Justifica tu criterio como ingeniero.

**Desafío 8: El Límite de Seguridad en la Torre**

Dos fuerzas de tensión actúan sobre un aislador de una torre de transmisión: $\vec{F}_1 = (500 \hat{i} + 1200 \hat{j}) \, \text{N}$ y $\vec{F}_2 = (900 \hat{i} + 1200 \hat{j}) \, \text{N}$.

- El Conflicto: El fabricante del aislador garantiza que este solo soporta una fuerza resultante máxima de $2.5 \, \text{kN}$.

- La Tarea: Calcula el módulo de la fuerza resultante. ¿Está el sistema operando en la zona de seguridad?

- El Veredicto: Como ingeniero supervisor, ¿autorizas la operación o exiges un refuerzo inmediato? .

**Desafío 9: La Maniobra del Dron de Mantenimiento**

Un dron de inspección de líneas debe ser lanzado con una velocidad de $22.2 \, \text{m/s}$ formando un ángulo de $62^\circ$ con la horizontal para evitar una descarga de arco eléctrico.

- El Conflicto: El dron necesita una velocidad vertical mínima de $18 \, \text{m/s}$ para estabilizarse antes de llegar a los cables.

- La Tarea: Calcula las componentes horizontal y vertical de la velocidad.

**Desafío 10: El Error de Logística en la Subestación**

Un técnico realiza tres desplazamientos sucesivos para localizar una falla en una red subterránea: $\vec{\Delta r}_1 = (400 \hat{i} + 300 \hat{j}) \, \text{m}$, $\vec{\Delta r}_2 = (-1000 \hat{i} + 800 \hat{j}) \, \text{m}$ y $\vec{\Delta r}_3 = (1400 \hat{i} - 1300 \hat{j}) \, \text{m}$.

- El Conflicto: El manual dice que la falla está a no más de $500 \, \text{m}$ en línea recta desde el punto de inicio.

- La Tarea: Calcula el módulo del desplazamiento total.

- La Reflexión: ¿Qué distancia total caminó el técnico (escalar) frente a qué tan lejos está realmente del inicio (vector)? ¿Por qué en ingeniería de mantenimiento "distancia" y "desplazamiento" pueden significar la diferencia entre encontrar una falla o perderse en el campo?

**Desafío 11: Eficiencia en el Plano Inclinado**

Se debe subir un transformador sobre un plano inclinado de $30^\circ$. Se aplica una fuerza de $500 \, \text{N}$ con un ángulo de $43^\circ$ respecto a la horizontal.

- El Conflicto: El operario cree que mientras más "hacia arriba" empuje, más fácil será el trabajo. Sin embargo, el ángulo real entre la fuerza y el camino (el plano) es lo que cuenta.

- La Tarea: Calcula el trabajo realizado. (Cuidado: Identifica correctamente el ángulo entre el vector fuerza y el vector desplazamiento).

- El Reto: ¿Bajo qué ángulo el trabajo desarrollado sería máximo? ¿Qué le recomendarías al operario para no desperdiciar energía?

**Desafío 12: Mesa de Fuerzas y Equilibrio Real**

- Desarrolla el experimento de la Mesa de Fuerzas y documenta lo siguiente en tu Diario de Aprendizaje:

- Conflicto Experimental: Al colocar las pesas en proporción 3, 4 y 5, ¿lograste el equilibrio perfecto a la primera?

- Evidencia: Inserta fotos donde se vea el anillo centrado y los ángulos medidos con el transportador.

- Tarea Crítica: Comprueba mediante el método de componentes si la suma vectorial de tus pesas reales da exactamente cero. Si no es así, ¿a qué le atribuyes la diferencia (fricción de las poleas, error de la balanza, etc.)?

- Mira algunos videos para ayudarte en el diseño y construcción de tu mesa de fuerzas:  

    - [Video 1](https://youtube.com/shorts/OuNLTRZL7ME?si=SjT5gfrGv1KCkZZs)
    - [Video 2](https://youtu.be/0TyVb26JNJk?si=7kiCcd18D6_5FYDj)
    - [Video 3](https://www.youtube.com/watch?v=NLVCpWGOWTs)

---
## 🎯 [¡Autoevaluate!](https://gemini.google.com/share/3c61a48a100e)
