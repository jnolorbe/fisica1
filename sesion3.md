# Sesión 3: Movimiento Rectilíneo II 

## Movimiento Rectilíneo Acelerado
---
## 📌 I. Fundamento Teórico
En esta sesión se tratan los conceptos de velocidad y aceleración instantánea como tasas de cambio temporales mediante el uso de derivadas e integrales. 

### 1. De la Posición a la Aceleración (Derivación)

Si conocemos la posición en función del tiempo $x(t)$ de una partícula, podemos saber la veleocidad y aceleración en función del tiempo:

* **Velocidad Instantánea:** Es la razón de cambio de la posición respecto al tiempo.
    $$v(t) = \frac{dx}{dt}$$
* **Aceleración Instantánea:** Es la razón de cambio de la velocidad respecto al tiempo.
    $$a(t) = \frac{dv}{dt} = \frac{d^2x}{dt^2}$$

### 2. De la Aceleración a la Posición (Integración)
Si conocemos la aceleración $a(t)$, podemos recuperar la velocidad $v(t)$ y luego la posición $x(t)$ mediante la integración:

* **De aceleración a velocidad:** 

$$v(t) = v_0 + \int_{0}^{t} a(t) dt$$

* **De velocidad a posición:** 

$$x(t) = x_0 + \int_{0}^{t} v(t) dt$$

> **💡 Regla de Oro:** Cuando la aceleración depende de la posición $a(x)$, usamos la identidad:
> $$ \int_{x_o}^{x} a(x) dx = \int_{v_o}^{v} v dv$$


---

## 🚀 II. Problemas Resueltos


### 🧩 Problema N° 1: El Carrete Lineal 
```{admonition} Análisis de Rapidez
:class: important
**Situación:** Un carrete lineal se mueve de un lado a otro según $x(t) = t^3 - 6t^2 + 9t$. El carrete siempre es impulsado al inicio con una velocidad inicial, se desplaza hacia la derecha y luego regresa a su punto de partida. Analizar los tramos en los que la partícula aumenta o disminuye su rapidez.
```

```{admonition} Solución
:class: dropdown hint
**1. Marco Teórico e Hipótesis Inicial:**
* **Ruta de la solución:** Hallar $v(t)$ y $a(t)$. La rapidez aumenta si $v \cdot a > 0$ y disminuye si $v \cdot a < 0$.
* **Predicción cualitativa:** Al ser impulsado, iniciará frenando hasta cambiar de sentido.

**2. Resolución Técnica:**
* **Velocidad:** $v(t) = 3t^2 - 12t + 9 = 3(t - 1)(t - 3)$. Ceros en $t=1$ y $t=3$.
* **Aceleración:** $a(t) = 6t - 12 = 6(t - 2)$. Cero en $t=2$.

**Análisis de Rapidez ($v \cdot a$):**
  * $t \in (0, 1)$: $v(+)$ y $a(-)$. El carrete avanza a la derecha y frena.
  * $t \in (1, 2)$: $v(-)$ y $a(-)$. El carrete regresa moviendose a la izquierda mientras gana rapidez.
  * $t \in (2, 3)$: $v(-)$ y $a(+)$. El carrete continua hacia la izquierda hasta detenerse.
  
**3. Discusión Crítica (Semáforo):**
* 🔴 **Rojo:** En $t=1$ y $t=3$ la rapidez es nula; un modelo real debe considerar el tiempo muerto de los relés de inversión de giro.
* 🟢 **Verde:** Identifica con precisión los puntos de retorno (límites del riel).
* 🔵 **Azul:** El instante $t=2$ es el punto de máxima velocidad de retorno.

**4. Análisis de Sensibilidad:**
Si el término cúbico fuera mayor, el carrete alcanzaría el punto de retorno mucho antes.

**5. Transferencia y Extensión:**
Este análisis es vital en el diseño de **actuadores lineales cíclicos**. El ingeniero debe asegurar que el frenado ocurra antes de llegar a los límites físicos para evitar el desgaste por impacto en los topes mecánicos.
```
---

### 🧩 Problema N° 2: El Sensor de Escaneado 
```{admonition} Función Exponencial
:class: important
**Situación:** Un cabezal de escaneo láser para inspección de paneles solares se desplaza según $x(t) = 10(1 - e^{-2t}) \, \text{m}$. Deducir la velocidad y aceleración cuando el tiempo es muy grande ($t \to \infty$).
```

```{admonition} Solución
:class: dropdown hint

**1. Marco Teórico e Hipótesis Inicial:**
* **Temática:** Cinemática de funciones trascendentes.
* **Ruta de la solución:** Derivación sucesiva y aplicación de límites.
* **Predicción cualitativa:** El cabezal debe frenar suavemente hasta detenerse en una posición límite.

**2. Resolución Técnica:**
* **Velocidad:** $v(t) = \frac{d}{dt} [10 - 10e^{-2t}] = 20e^{-2t} \, \text{m/s}$
* **Aceleración:** $a(t) = \frac{d}{dt} [20e^{-2t}] = -40e^{-2t} \, \text{m/s}^2$
* **Comportamiento Final:** $\lim_{t \to \infty} v(t) = 0$; $\lim_{t \to \infty} a(t) = 0$.

**3. Discusión Crítica (Semáforo):**
* 🔴 **Rojo:** Idealmente nunca llega a $10 \, \text{m}$, lo que en ingeniería eléctrica se conoce como error de estado estacionario.
* 🟢 **Verde:** Evita impactos bruscos (vibraciones) al final del recorrido.
* 🔵 **Azul:** La posición $x=10$ es la asíntota del sistema.

**4. Análisis de Sensibilidad:**
Si el exponente cambia a $-5t$, el cabezal responde más rápido, lo cual es crítico en líneas de producción de alta velocidad pero puede generar mayor estrés mecánico.

**5. Transferencia y Extensión:**
Este movimiento modela la **respuesta transitoria de un motor de corriente continua (DC)** de una faja transportadora, al arrancar. La velocidad del motor no alcanza su valor nominal instantáneamente, sino que sigue una curva de saturación similar para evitar movimientos bruscos.
```
---

### 🧩 Problema N° 3: Aceleración por Fuerza Magnética 
```{admonition} Aceleración en función de la velocidad $a(v)$
:class: important
**Situación:** Una partícula cargada en reposo en un acelerador lineal experimenta una fuerza que lo acelera $a = 4\sqrt{v} \, \text{m/s}^2$. Deducir su velocidad en función del tiempo si parte del reposo.
```
```{admonition} Solución
:class: dropdown hint

**1. Marco Teórico e Hipótesis Inicial:**
* **Temática:** Integración por separación de variables.
* **Ruta de la solución:** Sustituir $a = dv/dt$ y agrupar términos de velocidad.
* **Predicción:** La velocidad aumentará más rápido que en un movimiento rectilíneo uniformemente variado (MRUV).

**2. Resolución Técnica:**

$\frac{dv}{dt} = 4v^{1/2} \implies \int_{0}^{v} v^{-1/2} dv = \int_{0}^{t} 4 dt$

$2\sqrt{v} = 4t \implies v(t) = 4t^2 \, \text{m/s}$

**3. Discusión Crítica (Semáforo):**
* 🔴 **Rojo:** El modelo falla en $t=0$ si no hay una perturbación inicial: la velocidad y aceleración serían cero. Se requeriría una mínima velocidad inicial o perturbación para arrancar el movimiento.
* 🟢 **Verde:** Representa sistemas en los que conforme el cuerpo gana velocidad, retroalimenta positivamente la aceleración.
* 🔵 **Azul:** La aceleración resultante $a(t) = 8t$ indica que la fuerza requerida crece linealmente con el tiempo.

**4. Análisis de Sensibilidad:**
Una aceleración $a = 0.2\sqrt{v} \, \text{m/s}^2$ tiene una retroalimentación más suave, es decir el incremento de la acelración se hace cada vez con un menor ritmo.

**5. Transferencia y Extensión:**
Este modelo es fundamental para entender el movimiento lineal producido por **motores eléctricos de gran potencia**, donde buscamos que el acercamiento a la velocidad máxima de operación sea controlado para evitar picos de par mecánico.
```
---

## 📓 III. Actividades para el Portafolio Digital

Desarrolla los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques** (Marco Teórico, Resolución, Discusión Crítica de Semáforo, Análisis de Sensibilidad y Transferencia). Para el Portafolio digital solo presenta 4 Desafios.

**Desafío 1: El Brazo Robótico de Soldadura**
Un brazo robótico sigue la función $x(t) = t^3 - 9t^2 + 24t$.
* **El Reto:** Identifica los instantes donde la velocidad es nula.
* **Interpretación:** ¿Por qué un ingeniero debe evitar que el brazo se detenga bruscamente?

**Desafío 2: El Sensor de Presión de Aceite**
La posición de un émbolo sensor es $x(t) = \frac{10t}{t^2 + 4}$.
* **El Reto:** Determina el instante de máxima elongación y la velocidad en ese punto.
* **Análisis Crítico:** ¿Qué sucede con la velocidad cuando $t \to \infty$?

**Desafío 3: El Carrete de Bobinado Cíclico**
Un carrete lineal se mueve según $x(t) = 2t^3 - 15t^2 + 36t$.
* **El Reto:** Analiza los tramos de aumento y disminución de rapidez.
* **Toma de Decisión:** Si el carrete jala cobre y lo lleva hasta otro punto, ¿en qué tramos el estiramiento del cable corre más riesgo debido a cambios bruscos de rapidez? Justifica si recomendarías cambiar el motor por uno con un perfil de velocidad constante.

**Desafío 4: El Tren Maglev y el Frenado Dinámico**
Un tren experimenta una aceleración $a(v) = -0.5v$. Entra a la zona de estación a $v_0 = 20 \, \text{m/s}$.
* **El Reto:** Deduce la función de velocidad $v(t)$ integrando la expresión.
* **Análisis Técnico:** ¿Llegará el tren a detenerse por completo (v=0) en un tiempo finito según este modelo matemático? Compara la eficiencia de este frenado contra un freno de fricción mecánica de aceleración constante.

**Desafío 5: El Contactor Eléctrico**
Un contacto eléctrico tiene una aceleración dependiente de la posición $a(x) = 4x$. Parte de $x = 0.1 \, \text{m}$ con $v = 0$.
* **El Reto:** Encuentra la velocidad en función de la posición $v(x)$.
* **Interpretación Profesional:** En ingeniería eléctrica, la fuerza de atracción aumenta conforme los contactos se acercan. ¿Qué impacto tiene esta aceleración creciente en el desgaste de las caras de contacto por impacto?

**Desafío 6: El Actuador Magnético**
Un actuador magnético se desplaza sobre un riel lineal de baja fricción. Al desactivar el campo magnético impulsor, el dispositivo entra en una fase de frenado pasivo donde su velocidad decae según la función:
* **El Reto:** Determina la expresión de la aceleración $a(t)$.
* **Toma de Decisión:** Un técnico sugiere que el ventilador se detiene más rápido si se aplica un freno de contracorriente ($a = \text{constante}$). Basándote en el cálculo, ¿cuál modelo garantiza una parada más suave para evitar daños por fatiga en los rodamientos?

**Desafío 7: El Pulso de Corriente en un Solenoide**
Una partícula dentro de un campo variable tiene $v(t) = V_0(1 - e^{-t/\tau})$.
* **El Reto:** Halla las funciones de posición $x(t)$ y aceleración $a(t)$.
* **Análisis de Sensibilidad:** ¿Qué significa físicamente la constante de tiempo $\tau$? Si $\tau$ tiende a cero (respuesta instantánea), ¿qué sucede con el valor de la aceleración inicial y cómo afecta esto a la estructura mecánica del solenoide?

**Desafío 8: Oscilación de un Galvanómetro**
La aguja de un medidor analógico se mueve con $v(t) = A \cos(\omega t)$.
* **El Reto:** Halla la posición $x(t)$ asumiendo que parte del origen.
* **Interpretación Técnica:** ¿Qué relación existe entre los puntos de velocidad máxima y aceleración máxima? Explica por qué esto genera vibraciones que pueden descalibrar un instrumento de medición de alta precisión.

**Desafío 9: El Electrón en el Tubo de Rayos Catódicos**
Un electrón es acelerado con $a(t) = 10^{14} t \, \text{m/s}^2$ durante un microsegundo ($10^{-6} \, \text{s}$).
* **El Reto:** Calcula la velocidad final y la distancia recorrida en ese intervalo.
* **Evaluación:** Compara la distancia recorrida con el tamaño típico de un componente electrónico ($1 \, \text{cm}$). ¿Es este modelo de aceleración lineal adecuado o se requieren correcciones relativistas para distancias mayores?

**Desafío 10: La Cinta Transportadora de Mineral**
La aceleración de una cinta es $a(t) = 6t - 12$. En $t=0$, se conoce que $v_0 = 9 \, \text{m/s}$ y $x_0 = 0$.
* **El Reto:** Encuentra en qué instante la cinta vuelve a pasar por el origen de coordenadas.
* **Toma de Decisión:** Si la cinta transporta material frágil que se fractura con aceleraciones superiores a $10 \, \text{m/s}^2$, ¿en qué segundo exacto debe el ingeniero programar el limitador de potencia del motor para evitar pérdidas de material?

---