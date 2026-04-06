# Sesión 2: Cinemática Lineal (MRU, MRUV y Caída Libre)

---

## 📌 I. Fundamento Teórico

La cinemática describe el movimiento sin atender a sus causas. En esta sesión, nos enfocamos en el cambio de posición respecto al tiempo en una dimensión.

### 1. Movimiento Rectilíneo Uniforme (MRU)

Velocidad: Constante ($\vec{v} = \text{const}$).

Aceleración: Nula ($\vec{a} = 0$).

Ecuación: $x(t) = x_0 + v \cdot t$

### 2. Movimiento Rectilíneo Uniformemente Variado (MRUV)

Aceleración: Constante ($\vec{a} = \text{const}$).

Velocidad: Función lineal $v(t) = v_0 + a \cdot t$.

Posición: Función cuadrática $x(t) = x_0 + v_0 t + \frac{1}{2} a t^2$.

### 3. Caída Libre Vertical (CLV)

Caso especial de MRUV donde la aceleración es la gravedad ($g \approx 9.81 \, m/s^2$). Adoptamos el eje $+y$ hacia arriba, por lo tanto $\vec{a} = -g\hat{j}$.

---

## 📌 II. Problemas Resueltos

### Problema 1
```{admonition}  Movimiento Rectilíneo Uniforme
:class: important
Una particula se mueve en linea recta con velocidad constante, tal que su posición en función del tiempo es regsitrado en la tabla mostrada, deducir las ecuaciones cinemáticas del movimiento.

|  |  |  |  |  |  | 
|-----|-----|-----|-----|-----|-----|
| t(s) | 0.00 | 0.10 | 0.20 | 0.30 | 0.40 | 
| x(m) | 0.10 | 0.15 | 0.20 |0.25 | 0.30 | 

```

```{admonition} Solución
:class: dropdown hint

1. **Deducimos la ecuación de la posición en función del tiempo**. En la tabla se observa que el movil recorre distancias iguales en intervalos de tiempos iguales.  Se trata de un movimiento rectilíneo uniforme. En este caso, cada intervalo de tiempo de $0.10s$ recorre $0.05m$, su velocidad es constante $\vec{v} = 0.05m/0.10s = 0.50 \,m/s$. La posición en función del tiempo es una función lineal, considerando los valores de la tabla la ecuación de la posición esta dado por:

    $x = x_0 + \vec{v}t$

    Reemplazando, $x_0 = 0.10 \, m$ y $\vec{v} = + 0.50 \, m/s$:

    $x = 0.10 + 0.50 t$

2. ✨ **Sintésis:** La partícula hace un movimiento rectilíneo uniforme, con velocidad $0.50 \, m/s$. Las ecuaciones cinemáticas son:

    - $x = 0.10 + 0.50 t$

    - $\vec{v} = +0.50$

    - $\vec{a} = 0$

---
**Hazlo Tú**, Expresa las ecuaciones cinemáticas del MRU, tal que cumpla las siguientes condiciones:

a) $t = 0 \,s \, ; x_0 = 0 \, m \,;  v = 5 \, m/s $

b) $t = 0 \,s \, ; x_0 = 50 \, m \,;  v = -10 \, m/s $

c) $t = 0 \,s \, ; x_0 = -10 \, m \,;  v = 5 \, m/s $

---
```
---

### Problema 2
```{admonition}  Movimiento Uniformemente Acelerado
:class: important
En la figura se muestra la posición en función del tiempo de una partícula que se mueve en línea recta con aceleración constante. Expresar las ecuaciones cienmáticas del movimiento.


```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/cinematica01.png
:alt: cinematica
:width: 100%
:align: center
```

```{admonition} Solución
:class: dropdown hint

1. **Deducimos la ecuación de la posición en función del tiempo**. En la figura se observa que la distancia recorrida aumenta en $10 \, m$  cada segundo, nota que en el primer segundo recorre $5 \, m$, luego: $15 \, m$, $25 \, m$, $35 \, m$ y asi sucesivamente.  Se trata de un movimiento rectilíneo uniformemente variado, donde la rapidez aumenta uniformemente en $10 \, m/s$ cada segundo, es decir, con aceleración constante $\vec{a} = + 10 \, m/s^2$. Por lo tanto la posición en función del tiempo es una función cuadrática, considerando los valores de la figura la ecuación de la posición esta dado por:

    $x = x_0 + \vec{v}_0 t + \frac{1}{2} \vec{a}t^2$

    Reemplazando, $x_0 = 0\, m$ y $\vec{a} = + 10 \, m/s^2$:

    $x = 0 + \vec{v}_0 t + 5 t^2 $

    Para dar con la velocidad inicial reemplazamos alguna posición conocida en un instante dado, por ejemplo, para $t = 1.0 \,s$, $x = 5\, m$.

    $5 = \vec{v}_0 (1) + 5 (1)^2$

    De donde se deduce que la partícula parte del reposo:

    $\vec{v}_0 = 0$ 

    Finalmente, la posición en función del tiempo se expresa:

    $x = 5 t^2$

2. **Deducimos las ecuación de la velocidad en función del tiempo**. En un movimiento recitlineo uniformemente variado la velocidad es una función lineal del tiempo:

    $\vec{v} = \vec{v}_0 + \vec{a}t$

    Reemplazando, $v_0 = 0\, m/s$ y $\vec{a} = + 10 \, m/s^2$:

    $\vec{v} = 10t$

3. ✨ **Sintésis:** La partícula hace un movimiento rectilíneo uniformemente variado, parte del reposo y la velocidad aumenta en $10 \, m/s$ cada segundo. Las ecuaciones cinemáticas son:

    - $x = 5 t^2$

    - $\vec{v} = 10t$

    - $\vec{a} = +10$

---
**Hazlo Tú**, Expresa las ecuaciones cinemáticas de MRUV, tal que cumpla las siguientes condiciones:

a) $t = 0 \,s \, ; x_0 = 0 \, m \,;  v_0 = 5 \, m/s \, ; \vec{a} = 2 \, m/s^2$

b) $t = 0 \,s \, ; x_0 = 50 \, m \,;  v_0 = -10 \, m/s \, ; \vec{a} = -5 \, m/s^2$

c) $t = 0 \,s \, ; x_0 = -10 \, m \,;  v_0 = 0.50 \, m/s \, ; \vec{a} = 0.24 \, m/s^2$

---
```
---
### Problema 3

```{admonition} Movimiento Uniformemente Retardado 
:class: important

En la figura se muestra la posición en función del tiempo de una partícula que se mueve en línea recta con aceleración constante. Expresar las ecuaciones cienmáticas del movimiento. 

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/cinematica02.png
:alt: cinematica
:width: 100%
:align: center
```

```{admonition} Solución
:class: dropdown hint
1. ****Deducimos la ecuación de la posición en función del tiempo**. En este caso notamos que la distancia recorrida cada segundo disminuye en $10 \, m$ cada segundo, se trata entonces de un movimiento rectilíneo uniformemente variado, donde la rapidez disminuye uniformemente en $10 \, m/s$ cada segundo, es decir, con aceleración $\vec{a} = -10 \, m/s^2$. La posición en función del tiempo es una función cuadrática, considerando los valores de la figura la ecuación de la posición esta dado por:

    $ x = x_0 + \vec{v}_0 t + \frac{1}{2} \vec{a}t^2$

    Reemplazando, $x_0 = 50\, m$ y $\vec{a} = - 10 \, m/s^2$:

    $x = 50 + \vec{v}_0 t - 5 t^2 $

    Para dar con la velocidad inicial reemplazamos alguna posición de la figura, por ejemplo, para $t = 1.0 \,s$, $x = 125\, m$

    $125 = 50 + \vec{v}_0 (1) - 5 (1)^2$

    De donde se deduce que la partícula tiene una velocidad inicial de:

    $\vec{v}_0 = 80 \, m/s$ 

    Entonces la posicón en función del tiempo queda finalmente expresada:
    
    $x = 50 + 80t - 5 t^2$

2. **Deducimos la ecuación de la velocidad en función del tiempo**. En el movimiento recvtilíneo uniformemente variado, la velocidad en función del tiempo es una función lineal. 
    
    $\vec{v} = \vec{v}_0 +  \vec{a} t$

    Reemplazando, $\vec{v}_0 = 80 \, m/s$  y $\vec{a} = -10 \, m/s^2$.

    $\vec{v} = 80 - 10t$

    😮 _Esta ecuación tambien se puede deducir derivando la posición en función del tiempo_

3. **Sintesis**. La partícula hace un movimiento rectilíneo uniformemente variado, parte con $\vec{v}_0 = 80 \, m/s$ y la velocidad disminuye en $10 \, m/s$ cada segundo. Las ecuaciones cinemáticas son:

    - $x = 50 + 80t - 5 t^2$

    - $\vec{v} = 80 - 10t$

    - $\vec{a} = -10$

---
**Hazlo Tú**, Expresa las ecuaciones cinemáticas de MRUV retardado, tal que cumpla las siguientes condiciones:

a) $t = 0 \,s \, ; x_0 = 0 \, m \,;  v_0 = +60 \, m/s \, ; \vec{a} = -4 \, m/s^2$

b) $t = 0 \,s \, ; x_0 = 50 \, m \,;  v_0 = -54 \, m/s \, ; \vec{a} = +6 \, m/s^2$

c) $t = 0 \,s \, ; x_0 = -10 \, m \,;  v_0 = +2.50 \, m/s \, ; \vec{a} = -0.08 \, m/s^2$

---
```
--- 

### Problema 4
```{admonition}  Movimiento con aceleración constante
:class: important
Una partícula se mueve en linea recta, de modo que su posición varia en función del tiempo de acuerdo a la siguiente ecuación $x = 40t + 2t^2$, donde $x$ esta en metros y $t$ en segundos. Deducir la ecuación de la velocidad y de la aceleración usando límites.
```

```{admonition} Solución
:class: dropdown hint

1. **Deducimos la ecuación de la velocidad** usando límites.

    En el intervalo $t$ y $t + \Delta t$ las posiciones son:

    $x(t) = 40t + 2t^2$

    $x(t + \Delta t) = 40(t + \Delta t) + 2(t + \Delta t)^2 $

    Calulamos la velocidad media en el límite cuando $\Delta t\to 0$:

    $\vec{v} = \lim_{\Delta t\to 0} \frac{\Delta x}{\Delta t} = \lim_{\Delta t\to 0} \frac{x(t + \Delta t) - x(t)}{\Delta t}$

    $\vec{v} = \lim_{\Delta t\to 0} \frac{[40(t + \Delta t) + 2(t + \Delta t)^2] - [40t + 2t^2]}{\Delta t}$

    $\vec{v} = \lim_{\Delta t\to 0} \frac{40 \Delta t +  4 t \Delta t + \Delta t ^2}{\Delta t}$

    $\vec{v} = \lim_{\Delta t\to 0} (40 +  4 t  + \Delta t)$

    $\vec{v} = 40 +  4t  $

2. **Deducimos la ecuación de la aceleración** usando límites.

    En el intervalo $t$ y $t + \Delta t$ las velocidades son:

    $\vec{v}(t) = 40 + 4t $
  
    $\vec{v}(t + \Delta t) = 40 + 4(t + \Delta t)$

    Calulamos la aceleración media en el límite cuando $\Delta t\to 0$ de:

    $\vec{a} = \lim_{\Delta t\to 0} \frac{\vec{v}(t + \Delta t) - \vec{v}(t)}{\Delta t}$

    $\vec{a} = \lim_{\Delta t\to 0} \frac{[40 + 4(t + \Delta t)] - [40 + 4t]}{\Delta t}$

    $\vec{a} = \lim_{\Delta t\to 0} \frac{4 \Delta t}{\Delta t}$

    $\vec{a} = \lim_{\Delta t\to 0} (4)$

    $\vec{a} = 4 \, m/s^2 $

    😮 _La aceleración es constante, entonces el movimiento es rectilíneo uniformemente variado_

---
_✨ **Sintésis:** El cuerpo realiza un movimiento rectilíneo uniformemente variado, con una velocidad inicial de $\vec{v}(t) = 40 \, m/s$ y aceleración $\vec{a} = 4 \, m/s^2$. La deducción de la velocidad y la aceleración usando límites es un poco tediodosa y pueden ser deducidos usando reglas de derivación. 

---
```
---

### Problema 5

```{admonition} Movimiento de caída libre 
:class: important
Un cuerpo es lanzado verticalmente hacia arriba desde un acantilado de $20.0 \, m$ de alto, con una velocidad de $18.0 \, m/s$. La fricción con el aire hace que el movimiento hacia arriba tenga una aceleración constante de $-12.0 \, m/s^2$ y hacia abajo con $-8.0 \, m/s^2$. Deducir el tiempo que demora el cuerpo en llegar a la base del acantilado.

```


```{admonition} Solución
:class: dropdown hint
1. **Analizamos el tramo de subida**. Consideramos el origen de coordenadas en la base del acantilado      

    **Expresamos la posicón en función del tiempo**. Recordemos que la posición para un movimiento con aceleración constante es una función cuadrática con el tiempo:
    
    $y = y_0 + \vec{v}_0 t + \frac{1}{2} \vec{a}t^2$
    
    Reemplazmaos  $y_0 = 20.0$, $\vec{v}_0 = +18.0$ y  $\vec{a} = -12.0$:
    
    $ y = 20 + 18t - 6t^2$

    **Expresamos la ecuación de la velocidad**. Derivamos la posición en función del tiempo:

    $ \vec{v} = \frac{d}{dt} (20 + 18t - 6t^2) $

    $ \vec{v} = 18 - 12t$

    **Encontramos el instante cuando ha alcanzado su altura máxima**. En ese instante el cuerpo se detiene ($\vec{v} = 0$):

    $ 0 = 18 - 12t$

    $ t = 1.5 \, s$

    **Encontramos la altura máxima**. Esto ocurre en el instantee ($ t = 1.5\, s$):

    $ y_{max} = 20 + 18(1.5) - 6(1.5)^2$

    $ y_{max} = 33.5 \, m $

2. **Analizamos el tramo de bajada**. Consideramos el origen de coordenadas en la base del acantilado.    

    **Expresamos la posición en función del tiempo**. Aqui debes notar que la caída se da $1.5 \, s$ después de haber sido lanzado, por lo que la 
    ecuación de la posición se expresa:
    
    $y = y_0 + \vec{v}_0 (t - 1.5) + \frac{1}{2} \vec{a}(t-1.5)^2$

    Donde la posición inicial es el punto más alto $y_0 = 33.5 \, m$ y en ese instante el cuerpo parte del reposo $\vec{v}_0 = 0$, con una aceleración $\vec{a} = -8.0 \, m/s^2$.

    $y = 33.5 -4(t-1.5)^2$
    
    **Calulamos el tiempo que demora en llegar a la base del acantilado**. Cuando llega al acantilado $y = 0$:

    $0 = 33.5 -4(t-1.5)^2$

    $ t= 4.4 \, s$

---

_✨ **Sintésis:** El cuerpo sube disminuyendo su rapidez en $12 \, m/s$ cada segundo, hasta detenerse $\vec{v}_0 = 0$, esto ocurre en el instante $t = 1.5\, s$. Luego el cuerpo desciende aumentado su rapidez en $8 \, m/s$ cada segundo, hasta llegar al piso en el instante $t = 4.4\, s$._ 

---
```

---
### Problema 6

```{admonition} Movimiento de caída libre 
:class: important
Un bus que se mueve en línea recta entre un paradero y otro. Cuando el bus parte del paradero inicial, acelera con  $0.5 \, m/s^2$ hasta alcanzar una rapidez de $10.0 \, m/s$, el cuál mantiene constante durante $30 \, s$, instante en el que el conductor presiona los frenos y el bus desacelera con $2.5 \, m/s^2$ hasta detenerse en el paradero final. Expresar las ecuaciones cinemáticas.

```

```{admonition} Solución
:class: dropdown hint

1. **Analizamos el movimiento considerando tres tramos**. 

    **Tramo 1:**  Movimiento con aceleración constante, la ecuación de la posición esta dado por:

    $ x = x_0 + \vec{v}_0 t + \frac{1}{2} \vec{a}t^2$

    Reemplazamos los datos: $x_0 = 0$, $ \vec{v}_0 = 0$ y $\vec{a} = 0.5 \, m/s^2$. Nota que se ha considerado el origen de coordenadas en el paradero inicial y que el bus parte del reposo.

    $ x = 0.25t^2$

    La velocidad esta dado por la derivada de la posicón en función del tiempo:

    $ \vec{v} = \frac{d}{dt} (0.25t^2) $

    $ \vec{v} = 0.5t$

    Este tramo dura hasta alcanzar una velocidad de  $10.0 \, m/s$, esto ocurre en el instante $t = 20 \, s$. Al finalizar este tramo el bus se encontrará en $ x = 100 \, m$.

    **Tramo 2:**  Movimiento con velocidad constante, la posición en función del tiempo esta dado por:
    
    $ x = x_0 + \vec{v} t $

    Este tramo se inicia en $t = 20 \, s$,  en  $ x = 100 \, m$ con una velocidad  $\vec{v} = 10 \, m/s$, por lo tanto la ecuación de la posición es:

    $x = 100 + 10(t - 20)$

    Este tramo dura $30 \, s$, es decir, el cronómetro del observador registrará el instante $t = 50\, s$, en ese insatnte el bus se encontrará en la posición $x = 400\, m$.

    **Tramo 3:**  Movimiento con aceleración constante, la posición en función del tiempo esta dado por:
    
    $x = x_0 + \vec{v}_0 t + \frac{1}{2} \vec{a}t^2$ 

    Este tramo se inicia en $t = 50 \, s$,  en  $ x = 400 \, m$ con una velocidad inicial de $\vec{v} = 10 \, m/s$ y una aceleración de $\vec{a} = -2.5 \, m/s^2$,
    por lo tanto la ecuación de la posición es:

    $x = 400 + 10(t - 50) -1.25(t - 50)^2$.
    
    La velocidad esta dado por la derivada de la posicón en función del tiempo:
    
    $ \vec{v} = \frac{d}{dt} ( 400 + 10(t - 50) -1.25(t - 50)^2) $

    $ \vec{v} = 10 -2.5(t - 50)$

    Se detiene en el instante $t = 54 \, s$.
---

_✨ **Sintésis:** El bus realiza un MRUV acelerado, luego un MRU y termina con MRUV retardado, las ecuaciones de la posición son:_

    $x = 0.25t^2 \, \, t \le 30 $

    $ x = 100 + 10(t - 20) \, \, 30s \le t \le 50s $
    
    $x = 400 + 10(t - 50) -1.25(t - 50)^2 \, \, 50s \le t \le 54s $.

    _El movimiento completo dura $ 54\,s$_
---

```

---


## 💡 Ejercicios propuestos

1. En una carretera recta, un automóvil se desplaza con velocidad constante de $120 \, km/h$. En cierto instante, el automóvil pasa frente a una patrulla policial que se encuentra en reposo al costado de la vía. El conductor de la patrulla tarda $1.20 \, s$ en reaccionar antes de iniciar la persecución, A partir de ese momento, la patrulla parte desde el reposo y acelera con aceleración constante de $10  \, m/s^2$. Suponiendo que ambos vehículos se mueven en la misma dirección y en línea recta
¿Cuánto tiempo después de que el automóvil pasa frente a la patrulla es alcanzado por el patrullero?

2. En una carretera recta, dos vehículos se encuentran separados por una distancia de $500 \, m$. El Vehículo A parte del reposo y acelera con aceleración constante de 
$4 \, m/s^2$, en dirección hacia el Vehículo B. Simultáneamente, el Vehículo B se mueve hacia el Vehículo A con velocidad constante de $ 20 \, m/s$. Ambos se desplazan en la misma línea recta y uno frente al otro. ¿En qué posición ocurre el encuentro, medida desde el punto de partida del Vehículo A?


3. Dos trenes se mueven en direcciones opuestas por la misma vía. Los trenes parten simultáneamente de dos pueblos, $A$ y $B$, separados por una distancia $d$. Cada tren viaja uno hacia el otro con velocidad constante $v$. Una abeja se encuentra inicialmente delante del tren en $A$. Al salir el tren de $A$, la abeja viaja con una velocidad $u \lt v$ por la vía hacia $B$. Al encontrarse con el segundo tren, invierte instantáneamente su dirección hasta encontrarse con el primero, luego invierte de nuevo, etc. La abeja continúa volando entre los dos trenes hasta que es aplastada por el impacto. El propósito de este problema es calcular la distancia total recorrida por la abeja hasta ser aplastada. Considerar que la abeja es más rápida que los trenes. Hay al menos dos buenas maneras de resolver este problema. Una es calcular la distancia de cada tramo de vuelo y sumar la serie resultante. También hay otra manera de resolver el problema con muy pocos cálculos. Debes hacerlo de ambas maneras.

- Encuentra una expresión para la distancia dn recorrida por la abeja después de su enésimo encuentro con un tren. Define $d_0$ como la distancia recorrida durante el primer vuelo desde $A$ hacia el tren cerca de $B$, $d_1$ como la distancia recorrida por la abeja durante el primer viaje desde el tren de B hasta el tren de $A$, etc. Suma la serie resultante para obtener la respuesta final.
- Idea otra manera de obtener la misma respuesta con muy pocos cálculos.

4. Describe el movimiento de un bus que se mueve en línea recta entre un paradero y otro, considera una situación concreta, por ejemplo el movimiento de un bus que va desde la cuadra 10 hasta la cuadra 20 de la Av. La Marina. Asigna valores numéricos razonables. Describe el movimiento usando tus propias palabras utilizando los conceptos de velocidad y aceleración. Describe el movimiento usando ecuaciones. Describe el movimiento usando gráficas $x \, vs \, t$; $v \, vs. \, t$; $a \, vs. \, t$.  
Exprese la ecuación de la posición en función del tiempo.
Exprese la ecuación de la velocidad en función del tiempo.
Grafique la posición en función del tiempo.

5. Una partícula se mueve en linea recta tal que su posición es una función cúbica del tiempo, $x = 2(t -3)^3 + 54$. Analizar el movimiento y deducir el intervalo de tiempo cuando la rapidez de la particula aumenta o disminuye.

---

## 📝 Práctica Calificada N° 1: Cantidades Físicas y Vectores

🎯 Instrucciones Generales

Precisión Técnica: El uso de cifras significativas y unidades del Sistema Internacional (SI) es obligatorio en todas las respuestas.

Notación: Exprese los vectores utilizando vectores unitarios $(\hat{i}, \hat{j})$.


Criterio de Evaluación: Se valorará el planteamiento lógico antes que el resultado numérico final.

### 1. Operaciones con Cantidades Físicas (5 puntos)

En el laboratorio de circuitos, un estudiante mide la caída de tensión ($V$) y la corriente ($I$) en un resistor de carbón:

$V = 12.45 \, \text{V}$

$I = 2.3 \, \text{A}$

Se solicita:

- Determine el valor de la resistencia ($R$) mediante la ley de Ohm $R = \frac{V}{I}$. Exprese el resultado con el número correcto de cifras significativas.

- Si posteriormente se conecta en serie una resistencia de precisión de $0.156 \, \Omega$, calcule la resistencia total $R_{\text{total}} = R + 0.156 \, \Omega$. Aplique las reglas de suma para el redondeo final.

---

### 2. Descomposición Vectorial en el Plano (7 puntos)

Una antena de telecomunicaciones está sujeta por un cable que ejerce una fuerza de tensión $\vec{F_1}$ de magnitud $10.0 \, \text{N}$. La dirección del cable forma un ángulo de $143^\circ$ medido desde el eje $+x$ positivo en sentido antihorario.

Se solicita:

- Represente el vector $\vec{F_1}$ en términos de sus componentes rectangulares utilizando vectores unitarios $\hat{i}$ y $\hat{j}$.

- Análisis Crítico: Si el eje $x$ representa el suelo y el eje $y$ la torre vertical, ¿qué indica físicamente el signo de la componente horizontal en este sistema de referencia?

(Datos: $\sin(143^\circ) \approx 0.60$; $\cos(143^\circ) \approx -0.80$)

---

### 3. Suma de Fuerzas Electromagnéticas (8 puntos)

Dos fuerzas de origen magnético actúan sobre una partícula cargada en el origen de coordenadas:

$\vec{A} = (4.0\hat{i} - 2.0\hat{j}) \, \text{mN}$

$\vec{B}$ es un vector de magnitud $5.0 \, \text{mN}$ que apunta directamente en la dirección del eje $+y$.

Se solicita:

- Calcule el vector resultante $\vec{R} = \vec{A} + \vec{B}$ en forma de componentes.

- Determine la magnitud (módulo) de $\vec{R}$ y el ángulo $\theta$ que forma con el eje $+x$

---

