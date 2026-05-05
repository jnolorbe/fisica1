# Sesión 4: Movimiento Curvilíneo 

## 📌 I. Fundamento Teórico
En esta sesión se estudian las trayectorias curvas de las partículas en dos dimensiones, analizando el movimiento mediante vectores posición, velocidad y aceleración. Se abordan tres casos fundamentales: movimiento general en 2D, movimiento de proyectiles bajo gravedad, y movimiento circular con sus variantes.

### 1.1 Movimiento en Dos Dimensiones

Cuando una partícula se mueve en un plano, su posición, velocidad y aceleración tienen dos componentes. En un movimiento curvilíoneo, el vector posición $\vec{r}(t)$ se traza desde el origen de coordenadas hasta la posición de la partícula. El vector velocidad $\vec{v}(t)$ es tangente a la trayectoria y el vector aceleración $\vec{a}(t)$ se dirige hacia el interior de la concavidad de la curva. El analisis del movimento puede llevarse a cabo de forma independiente con cada componente.

- El **vector de posición** se expresa con sus dos compontentes que dependen del tiempo:

$$\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}$$


* El **vector Velocidad:** Es la derivada temporal del vector de posición.

$$\vec{v}(t) = \frac{d\vec{r}}{dt} = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j} = v_x\hat{i} + v_y\hat{j}$$
    
- La magnitud de la velocidad (rapidez) es:

  $$v = |\vec{v}| = \sqrt{v_x^2 + v_y^2}$$

* El **Vector Aceleración:** Es la derivada temporal del vector de velocidad.

$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{dv_x}{dt}\hat{i} + \frac{dv_y}{dt}\hat{j} = a_x\hat{i} + a_y\hat{j}$$

- La magnitud de la aceleración es:

  $$a = |\vec{a}| = \sqrt{a_x^2 + a_y^2}$$


> **💡 Componentes Intrínsecas:** La aceleración puede descomponerse en:
> * **Aceleración tangencial** ($a_t$): Mide el cambio de la magnitud de la velocidad.
>   $$a_t = \frac{dv}{dt}$$
> * **Aceleración normal/centrípeta** ($a_n$): Mide el cambio de la dirección de la velocidad.
>   $$a_n = \frac{v^2}{\rho}$$
>   donde $\rho$ es el radio de curvatura de la trayectoria.

### 1.2. Movimiento de Proyectiles

El movimiento de un proyectil bajo la gravedad terrestre (despreciando la resistencia del aire) es un caso particular de movimiento en 2D donde:

* **Aceleración:** $\vec{a} = -g\hat{j}$ (constante, dirigida hacia abajo)

* **Condiciones iniciales:** El proyectil es disparado con una velcoidad $\vec{v}_0$ qué forma un ángulo $\theta$ con la horizontal, de modo que sus componentes son:

    - $\vec{v}_x = v_0\cos\theta\,\hat{i}$

    - $\vec{v}_y = v_0\sin\theta\,\hat{j}$

**Ecuaciones cinemáticas desacopladas:**

| Eje X | Eje Y |
|---------------------------|------------------------------------------|
| $a_x = 0$ | $a_y = -g$ |
| $v_x = v_0\cos\theta$ | $v_y = v_0\sin\theta - gt$ |
| $x = (v_0\cos\theta)t$ | $y = (v_0\sin\theta)t - \frac{1}{2}gt^2$ |

**Ecuación de la trayectoria** 

Eliminando el tiempo $t$ al combinar las ecuaciones paramétricas de la posicion $x(t)$ e $y(t)$, se obtiene la ecuación cartesiana de la trayectoria:

$$y = x\tan\theta - \frac{gx^2}{2v_0^2\cos^2\theta}$$

**Parámetros importantes:**

* **Alcance horizontal máximo:** $R = \frac{v_0^2\sin(2\theta)}{g}$ (ocurre cuando $\theta = 45°$)
* **Altura máxima:** $H = \frac{v_0^2\sin^2\theta}{2g}$
* **Tiempo de vuelo:** $T = \frac{2v_0\sin\theta}{g}$
* **Angulos complementarios:** Dos angulos complementariso tienen el mismo alcance horizontal.

> **💡 Regla de Oro:** En el punto más alto de la trayectoria, $v_y = 0$, pero la velocidad nunca es cero (siempre conserva la componente horizontal $v_x$).

### 1.3. Movimiento Circular

Cuando una partícula describe una trayectoria circular de radio $R$:

#### Movimiento Circular Uniforme (MCU)
La rapidez es constante, pero la dirección de la velocidad cambia continuamente.

* **Velocidad angular:** $\omega = \frac{d\theta}{dt}$ (constante en MCU)
* **Velocidad tangencial:** $v = \omega R$
* **Aceleración centrípeta:** $a_c = \omega^2 R = \frac{v^2}{R}$

#### Movimiento Circular Uniformemente Variado (MCUV)
La rapidez angular varía con el tiempo.

* **Aceleración angular:** $\alpha = \frac{d\omega}{dt} = \frac{d^2\theta}{dt^2}$
* **Ecuaciones cinemáticas (análogas al MRUV):**
  $$\omega = \omega_0 + \alpha t$$
  $$\theta = \theta_0 + \omega_0 t + \frac{1}{2}\alpha t^2$$
  $$\omega^2 = \omega_0^2 + 2\alpha(\theta - \theta_0)$$

* **Aceleración total:** Tiene dos componentes perpendiculares:
  $$\vec{a} = \vec{a}_t + \vec{a}_c$$
  
  donde:
  * $a_t = \alpha R$ (tangencial, cambia la magnitud de $v$)
  * $a_c = \omega^2 R = \frac{v^2}{R}$ (centrípeta, cambia la dirección de $v$)
  
  La magnitud de la aceleración total es:
  $$a = \sqrt{a_t^2 + a_c^2}$$

> **💡 Regla de Oro:** En MCUV, la aceleración total nunca es puramente centrípeta ni puramente tangencial (excepto en los instantes donde una de las componentes se anula).

---

## 🚀 II. Problemas Resueltos

### 🧩 Problema N° 1
```{admonition} Movimiento de un Nadador al Cruzar un Río
:class: important
Un nadador quiere cruzar un río de ancho $d_1 = 50$ m. La máxima rapidez con la que el nadador nada en aguas calmadas (sin corrientes) es $u_s = 1.2$ m/s. La corriente del río fluye con rapidez $v_c = 0.8$ m/s. Determinar: 

- (a) la rapidez resultante del nadador respecto a la orilla, cuando nade perpendicular al río, $\theta = 0$. 

- (b) el tiempo que tarda en cruzar. 

- (c) la distancia que es arrastrado río abajo, cuando nade perpendicular al río, $\theta = 0$

- (d) el ángulo $\theta$ con el que debe nadar para llegar exactamente al punto frente a su partida.

```{figure} /figuras/s04_fig3.png
:width: 40%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Analizar las velocidades como vectores. La velocidad del nadador respecto a la orilla es la suma vectorial de su velocidad respecto al agua más la velocidad de arrastre de la corriente.
* **Predicción cualitativa:** El nadador será arrastrado río abajo. Para llegar al punto frente al inicio, debe compensar la corriente nadando ligeramente contra ella.

**2. Resolución:**

* **Sistema de referencia:** Eje X horizontal (dirección de la corriente), Eje Y vertical (cruzando el río).

* **Velocidad del nadador respecto al agua:** $\vec{v}_{n/a} = 1.2\hat{j}$ m/s
* **Velocidad de la corriente:** $\vec{v}_{c} = 0.8\hat{i}$ m/s

**(a) Velocidad resultante respecto a la orilla:**
$$\vec{v}_{n/o} = \vec{v}_{n/a} + \vec{v}_{c} = 0.8\hat{i} + 1.2\hat{j} \text{ m/s}$$

$$v_{n/o} = \sqrt{0.8^2 + 1.2^2} = \sqrt{0.64 + 1.44} = \sqrt{2.08} \approx 1.44 \text{ m/s}$$

**(b) Tiempo de cruce:**
El tiempo depende solo de la componente perpendicular (cruce efectivo):
$$t = \frac{D}{v_{n/a}} = \frac{50}{1.2} \approx 41.67 \text{ s}$$

**(c) Distancia arrastrada río abajo:**
$$d = v_c \cdot t = 0.8 \times 41.67 \approx 33.33 \text{ m}$$

**(d) Ángulo de compensación:**
Para que la componente X sea nula: $v_{n/a}\sin\theta = v_c$
$$\sin\theta = \frac{0.8}{1.2} = 0.667 \Rightarrow \theta = \arcsin(0.667) \approx 41.8°$$

El nadador debe orientarse $41.8°$ contra la corriente (aguas arriba).

**3. Discusión Crítica:**
* El tiempo de cruce no depende de la corriente cuando nada perpendicularmente; solo la componente perpendicular al río importa para el cruce.
* En un río real con velocidad variable (mayor en el centro), la trayectoria sería curva, no rectilínea.
* La compensación de $41.8°$ requiere que $v_n > v_c$; si la corriente fuera más rápida que el nadador, sería imposible llegar al punto frente al inicio.

**4. Análisis de Sensibilidad:**
Si la corriente aumenta un 50% ($v_c = 1.2$ m/s), el ángulo de compensación sería de $90°$ (nadando completamente contra la corriente), haciendo imposible el cruce perpendicular en tiempo finito.

**5. Extensión:**
Este análisis es fundamental en la navegación de embarcaciones y en el diseño de trayectorias de vehículos aéreos (corrección por viento cruzado). Los sistemas de piloto automático calculan continuamente este ángulo de deriva.

```
---

### 🧩 Problema N° 2
```{admonition} Movimiento de un Proyectil Lanzado Horizontalmente
:class: important
Un caza militar vuela horizontalmente a $v_0 = 1800$ km/h (500 m/s) y a una altura $h = 3000$ m sobre el objetivo. En el instante $t = 0$ suelta una bomba para impactar un blanco terrestre. Despreciando los efectos del aire y de la rotación de la Tierra, deducir: 

- (a) el tiempo que tarda la bomba en llegar al suelo.

- (b) la distancia horizontal recorrida desde el punto de soltado hasta el impacto.

- (c) la velocidad del proyectil justo antes del impacto

- (d) el ángulo de impacto respecto a la horizontal.

- (e) la distancia horizontal entre el avión y la bomba en el instante del impacto.
 

```{figure} /figuras/s04_fig4.jpg
:width: 40%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** El movimiento horizontal es sin aceleración ($a_x = 0$) y el vertical es caída libre ($a_y = -g$). Las condiciones iniciales son $v_{0x} = 500$ m/s y $v_{0y} = 0$.
* **Predicción cualitativa:** La trayectoria será una parábola muy "achatada" debido a la alta velocidad horizontal. El avión y la bomba comparten la misma velocidad horizontal inicial, por lo que el avión estará directamente sobre la bomba en todo momento (sin resistencia del aire).

**2. Resolución:**

**(a) Tiempo de caída:**
Desde $y = h - \frac{1}{2}gt^2$, cuando $y = 0$:
$$0 = 3000 - \frac{1}{2}(9.8)t^2$$
$$t = \sqrt{\frac{2 \times 3000}{9.8}} = \sqrt{612.24} \approx 24.74 \text{ s}$$

**(b) Alcance horizontal:**

$$x = v_{0x} \cdot t = 500 \times 24.74 = 12370 \text{ m} \approx 12.37 \text{ km}$$

**(c) Velocidad antes del impacto:**

* Componente horizontal: $v_x = v_{0x} = 500$ m/s (constante, sin resistencia del aire)
* Componente vertical: $v_y = -gt = -9.8 \times 24.74 \approx -242.45$ m/s

$$v = \sqrt{500^2 + (-242.45)^2} = \sqrt{250000 + 58782} = \sqrt{308782} \approx 555.7 \text{ m/s}$$

> **Conversión:** $555.7$ m/s $\approx 2000$ km/h, cercano a Mach 1.6 a nivel del mar.

**(d) Ángulo de impacto:**
$$\tan\theta = \frac{|v_y|}{v_x} = \frac{242.45}{500} = 0.485$$
$$\theta = \arctan(0.485) \approx 25.9° \text{ bajo la horizontal}$$

**(e) Posición relativa avión-bomba:**
Sin resistencia del aire, la bomba conserva la velocidad horizontal del avión. Por lo tanto, en todo instante:
$$x_{bomba}(t) = x_{avion}(t)$$

En el momento del impacto, el avión está exactamente sobre el punto de impacto a 3000 m de altura, habiendo recorrido la misma distancia horizontal (12.37 km).

**3. Discusión Crítica:**
* **Efecto de la resistencia del aire:** A 500 m/s (Mach ~1.5), la resistencia del aire es extremadamente significativa. El avion experimentaria una aceleración horizontal de frenado y una aceleración vertical menor a ala de la aceleraicón gravitatorioa. El alcance sería menor y el tiempo de caída ligeramente mayor.
* **Punto de mira:** Los sistemas de puntería calculan el "tiempo de caída" y la "distancia de adelantamiento" (12.37 km en este caso). El bombardero debe soltar la bomba mucho antes de sobrevolar el objetivo.

**4. Análisis de Sensibilidad:**

* Si el efecto del aire redujera la aceleración gravitatoria en un 2% (9.6 m/s²), el tiempo de caída aumentaría a 25.00 s, a penas unos 0.26 s adicionales, pero tendría un efecto en el alcance horizontal, con un error de 130 m lejos del blanco.

* El alcance horizontal, tamnbién puede ser modificado si la bomba se deja caer de diferentes alturas. La altura tiene un efecto no lineal; duplicar la altura solo aumenta el alcance un 41%, mientras que duplicar la velocidad del avión duplica el alcance.

**5. Extensión:**
* **Bombas inteligentes (JDAM):** Incorporan alas y sistemas GPS que permiten correcciones de trayectoria en vuelo, compensando errores de lanzamiento y resistencia del aire.
* **Comparación histórica:** En la Segunda Guerra Mundial, los bombarderos B-17 volaban a ~400 km/h y bombardeaban desde 8000 m. Los tiempos de caída superaban los 40 s, requiriendo complejos cálculos de puntería con computadoras mecánicas (Norden bombsight)
```
---

### 🧩 Problema N° 3
```{admonition} Movimiento de Proyectil Disparado en una Superficie Plana
:class: important
Durante el siglo XVIII, el Fuerte Real Felipe del Callao protegía el principal puerto del Virreinato del Perú de incursiones piratas y corsarias. Sus cañones de bronce disparaban balas de cañón de hierro con velocidad inicial $v_0 = 250$ m/s desde el nivel del mar ($y_0 = 0$) con un ángulo de elevación ajustable. Deducir:.

- (a) el ángulo de alcance máximo para interceptar naves enemigas.

- (b) la altura máxima alcanzada por el proyectil cuando se dispara a $\theta = 35°$.

- (c) el tiempo de vuelo para $\theta = 35°$

- (d) la ecuación de la trayectoria para este ángulo.

- (e) si un cañón posicionado en la muralla a $15$ m sobre el nivel del mar puede alcanzar una goleta pirata anclada a $4$ km de distancia disparando a $40°$.
 

```{figure} /figuras/s04_fig6.jpeg
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Usar las ecuaciones del movimiento de proyectiles con $y_0 = 0$ y condiciones de simetría para superficie plana. 
* **Predicción cualitativa:** El alcance máximo debería ocurrir a $45°$ por simetría. Desde la muralla del Real Felipe (15 m de altura), el proyectil tiene ventaja gravitacional adicional, permitiendo alcances mayores que desde el nivel del mar.

**2. Resolución:**

**(a) Ángulo para alcance máximo desde nivel del mar:**
$$R = \frac{v_0^2\sin(2\theta)}{g}$$

Para maximizar $R$, $\sin(2\theta) = 1 \Rightarrow 2\theta = 90° \Rightarrow \theta = 45°$

$$R_{max} = \frac{250^2 \times 1}{9.8} = \frac{62500}{9.8} \approx 6377.6 \text{ m} \approx 6.38 \text{ km}$$

> **Contexto histórico:** Los cañones del Real Felipe tenían un alcance efectivo de 2-3 km debido a la resistencia del aire y la imprecisión de la pólvora negra. El alcance teórico de 6.4 km era inalcanzable en condiciones reales de combate.

**(b) Altura máxima para $\theta = 35°$:**
$$H = \frac{v_0^2\sin^2\theta}{2g} = \frac{62500 \times \sin^2(35°)}{2 \times 9.8} = \frac{62500 \times 0.3289}{19.6}$$

$$H = \frac{20558.6}{19.6} \approx 1048.9 \text{ m} \approx 1.05 \text{ km}$$

> **Nota:** Esta altura supera la altura de vuelo de muchas aves marinas y permitía a los artilleros observar la caída del proyectil contra el mástil de los barcos enemigos.

**(c) Tiempo de vuelo para $\theta = 35°$:**
$$T = \frac{2v_0\sin\theta}{g} = \frac{2 \times 250 \times \sin(35°)}{9.8} = \frac{500 \times 0.5736}{9.8}$$

$$T = \frac{286.8}{9.8} \approx 29.27 \text{ s}$$

> **Táctica naval:** En 29 segundos, una goleta pirata a 5 nudos (2.57 m/s) podría desplazarse ~75 m. Los artilleros debían "apuntar por anticipación", calculando la posición futura del blanco.

**(d) Ecuación de la trayectoria para $\theta = 35°$:**
$$y = x\tan\theta - \frac{gx^2}{2v_0^2\cos^2\theta}$$

$$y = x\tan(35°) - \frac{9.8x^2}{2 \times 62500 \times \cos^2(35°)}$$

$$y = 0.700x - \frac{9.8x^2}{125000 \times 0.671} = 0.700x - \frac{9.8x^2}{83875}$$

$$y = 0.700x - 1.168 \times 10^{-4}x^2$$

donde $x$ e $y$ están en metros.

**(e) Alcance desde la muralla del Real Felipe:**
Desde $y_0 = 15$ m, $\theta = 40°$, blanco a $x = 4000$ m.

Ecuación de trayectoria con altura inicial:
$$y = y_0 + x\tan\theta - \frac{gx^2}{2v_0^2\cos^2\theta}$$

$$y = 15 + 4000\tan(40°) - \frac{9.8 \times 4000^2}{2 \times 62500 \times \cos^2(40°)}$$

$$y = 15 + 4000 \times 0.839 - \frac{9.8 \times 16 \times 10^6}{125000 \times 0.587}$$

$$y = 15 + 3356 - \frac{1.568 \times 10^8}{73375} = 15 + 3356 - 2137.4$$

$$y = 1233.6 \text{ m}$$

**Conclusión:** El proyectil pasa a 1233.6 m **sobre** el blanco. La goleta está en $y = 0$, por lo que el proyectil la sobrepasa ampliamente.

**¿A qué distancia impacta realmente?**
Resolviendo $y = 0$:
$$0 = 15 + x\tan(40°) - \frac{9.8x^2}{2 \times 62500 \times \cos^2(40°)}$$

$$0 = 15 + 0.839x - 1.168 \times 10^{-4}x^2$$

Ecuación cuadrática: $1.168 \times 10^{-4}x^2 - 0.839x - 15 = 0$

$$x = \frac{0.839 + \sqrt{0.839^2 + 4 \times 1.168 \times 10^{-4} \times 15}}{2 \times 1.168 \times 10^{-4}}$$

$$x = \frac{0.839 + \sqrt{0.704 + 0.007}}{2.336 \times 10^{-4}} = \frac{0.839 + 0.843}{2.336 \times 10^{-4}}$$

$$x \approx \frac{1.682}{2.336 \times 10^{-4}} \approx 7200 \text{ m} = 7.2 \text{ km}$$

> **Verificación táctica:** Desde 15 m de altura a $40°$, el alcance es ~7.2 km, superando ampliamente los 4 km de la goleta. El artillero debería reducir el ángulo a aproximadamente $25°$ para impactar a 4 km.

**3. Discusión Crítica:**
* **Resistencia del aire:** A 250 m/s, una bala de cañón de 6 kg experimenta una fuerza de arrastre considerable. En la realidad, el alcance efectivo se reducía significativamente. La pólvora negra del siglo XVIII producía velocidades iniciales variables (±20%) debido a la humedad y la granulometría irregular.

**4. Análisis de Sensibilidad:**

* **Ángulo de disparo:** Una variación ligera del ángulo de lanzamiento, por ejemplo de 40° a 35° (una variación de -5°), el alcance disminuye en un -12% (~6.3 km).
* **Velocidad inicial:** Una variación del 10 % en la velocidad de disparo, por ejemplo de 250 m/s a 225 m/s (una variación de -10% ), el alcance disminuye en un -19% (~5.8 km).
* **Altura de muralla:** Una variación en la altura del disparo, por ejemplo disparar a 25 m de alto en lugar de a 15m (una variación de + 10 m),  el alcance aumenta en un +2% (~7.3 km).

**5. Extensión:**
* **El Real Felipe hoy:** El fuerte, construido entre 1747-1774, es el único baluarte de defensa virreinal intacto en América. Sus murallas de 10 m de grosor resistieron el bombardeo de la flota española durante la independencia (1821) y el ataque de la flota chilena en la Guerra del Pacífico (1880).
* **Balística forense:** Los arqueólogos han recuperado balas de cañón incrustadas en las murallas. Analizando su deformación, estiman velocidades de impacto de 150-180 m/s, consistentes con nuestro modelo incluyendo resistencia del aire.
* **Ingeniería de fortificaciones:** El diseñador francés Louis Godín diseñó el Real Felipe siguiendo principios de Vauban. La disposición estrellada permitía fuego cruzado desde múltiples ángulos, eliminando "puntos ciegos" donde los piratas podrían anclar fuera del alcance de un solo cañón.
```
---

### 🧩 Problema N° 4

```{admonition} Movimiento de un Proyectil en un Plano Inclinado
:class: important
Desde la base de un plano inclinado con ángulo $\alpha = 20°$ respecto a la horizontal, se dispara un proyectil con $v_0 = 25$ m/s y ángulo $\theta = 50°$ respecto a la horizontal. El plano inclinado asciende desde el punto de disparo. Calcular:

- (a) el tiempo de impacto con el plano.

- (b) la distancia recorrida sobre el plano.

- (c) demostrar que el ángulo de alcance máximo sobre el plano inclinado es $\theta_{max} = 45° + \frac{\alpha}{2}$

```{figure} /figuras/s04_fig7.png
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Plantear las ecuaciones del proyectil y la recta del plano inclinado ($y = x\tan\alpha$). Encontrar la intersección y expresar el alcance en función del ángulo de disparo.
* **Predicción cualitativa:** El proyectil impactará el plano antes de completar su trayectoria parabólica completa. El ángulo óptimo debería ser mayor que $45°$ para compensar la pendiente ascendente.

**2. Resolución:**

**Ecuaciones del proyectil:**
$$x = (v_0\cos\theta)t$$
$$y = (v_0\sin\theta)t - \frac{1}{2}gt^2$$

**Ecuación del plano inclinado:**
$$y = x\tan\alpha$$

**(a) Tiempo de impacto:**
Igualando las $y$:
$$(v_0\sin\theta)t - \frac{1}{2}gt^2 = (v_0\cos\theta)t\tan\alpha$$

$$v_0\sin\theta - \frac{1}{2}gt = v_0\cos\theta\tan\alpha$$

$$t = \frac{2v_0(\sin\theta - \cos\theta\tan\alpha)}{g} = \frac{2v_0\cos\theta(\tan\theta - \tan\alpha)}{g}$$

Sustituyendo valores ($\theta = 50°$, $\alpha = 20°$):
$$t = \frac{2 \times 25 \times \cos(50°) \times (\tan(50°) - \tan(20°))}{9.8}$$
$$t = \frac{50 \times 0.643 \times (1.192 - 0.364)}{9.8} = \frac{50 \times 0.643 \times 0.828}{9.8} \approx 2.72 \text{ s}$$

**(b) Distancia sobre el plano:**
$$x = v_0\cos\theta \cdot t = 25 \times \cos(50°) \times 2.72 \approx 25 \times 0.643 \times 2.72 \approx 43.7 \text{ m}$$

$$d = \frac{x}{\cos\alpha} = \frac{43.7}{\cos(20°)} = \frac{43.7}{0.94} \approx 46.5 \text{ m}$$

**(c) Ángulo de alcance máximo:**
El alcance sobre el plano es:
$$R = \frac{2v_0^2\cos\theta\sin(\theta - \alpha)}{g\cos^2\alpha}$$

Para maximizar, derivamos respecto a $\theta$ e igualamos a cero:
$$\frac{dR}{d\theta} = 0 \Rightarrow \cos(2\theta - \alpha) = 0$$

$$2\theta - \alpha = 90° \Rightarrow \theta_{max} = 45° + \frac{\alpha}{2}$$

Para $\alpha = 20°$: $\theta_{max} = 45° + 10° = 55°$

**3. Discusión Crítica:**
* El ángulo óptimo sobre un plano inclinado ascendente es mayor que $45°$ porque se necesita más componente vertical para compensar la pendiente.
* Para un plano descendente, el ángulo óptimo sería $\theta_{max} = 45° - \frac{|\alpha|}{2}$.
* El tiempo de vuelo es menor que en superficie plana porque el proyectil encuentra el suelo antes.

**4. Análisis de Sensibilidad:**
Si el ángulo del plano aumenta a $30°$, el ángulo óptimo de disparo sería $60°$. El alcance máximo disminuye porque la componente efectiva de la gravedad a lo largo del plano aumenta.

**5. Extensión:**
Este modelo aplica en minería a cielo abierto para calcular parámetros de voladura, en diseño de rampas de esquí para saltos, y en balística militar para disparos en terreno montañoso.
```
---

### 🧩 Problema N° 5

```{admonition} Movimiento Circular de una Partícula Cargada
:class: important
En una cámara de burbujas de física de partículas, se observan diferentes trayectorias circulares de diferentes particulas cargadas debido a la acción de campo magnéticos. La trayectoria queda registrada para algunas particulas como arcos de circunferencia, otras como una espiral y algunas quedan atrapadas en la cámara haciendo un movimeinto circular uniforme. La foto muestra a un electrón en una trayectoria circular de radio $R = 15$ cm con rapidez constante $v = 2.5 \times 10^7$ m/s. Determinar: (, , , , , y 

- (a) la velocidad angular del electrón.

- (b) el período de revolución.

- (c) la frecuencia de rotación.

- (d) la aceleración centrípeta y compararla con $g$.

- (e) el número de vueltas completadas en $1$ microsegundo.

- (f) la distancia total recorrida en ese intervalo.


```{figure} /figuras/s04_fig8.png
:width: 50%
:align: center
```

```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Aplicar las ecuaciones cinemáticas del MCU: $\omega = v/R$, $T = 2\pi/\omega$, $a_c = v^2/R$. El movimiento es uniforme porque la rapidez es constante; solo cambia la dirección de la velocidad.
* **Predicción cualitativa:** A velocidades tan altas, el período será extremadamente corto (nanosegundos) y la aceleración centrípeta enorme (miles de millones de $g$). 
**2. Resolución:**

**Datos:**
* $R = 0.15$ m
* $v = 2.5 \times 10^7$ m/s (constante, MCU)

**(a) Velocidad angular:**
$$\omega = \frac{v}{R} = \frac{2.5 \times 10^7}{0.15} = 1.667 \times 10^8 \text{ rad/s}$$

> **Conversión:** $\omega \approx 1.67 \times 10^8$ rad/s $\approx 2.65 \times 10^7$ rev/s

**(b) Período de revolución:**
$$T = \frac{2\pi}{\omega} = \frac{2\pi R}{v} = \frac{2\pi \times 0.15}{2.5 \times 10^7}$$

$$T = \frac{0.9425}{2.5 \times 10^7} = 3.77 \times 10^{-8} \text{ s} = 37.7 \text{ ns}$$

> **Contexto:** En 37.7 nanosegundos, la luz recorre ~11.3 m. El electrón completa una vuelta en este tiempo.

**(c) Frecuencia de rotación:**
$$f = \frac{1}{T} = \frac{\omega}{2\pi} = \frac{1.667 \times 10^8}{2\pi} \approx 2.653 \times 10^7 \text{ Hz} = 26.53 \text{ MHz}$$

> **Nota:** Esta frecuencia está en la banda de radiofrecuencia (HF). En aceleradores reales, las frecuencias de RF para sincronización están en este rango.

**(d) Aceleración centrípeta:**
$$a_c = \frac{v^2}{R} = \frac{(2.5 \times 10^7)^2}{0.15} = \frac{6.25 \times 10^{14}}{0.15}$$

$$a_c = 4.167 \times 10^{15} \text{ m/s}^2$$

**Comparación con $g$:**
$$\frac{a_c}{g} = \frac{4.167 \times 10^{15}}{9.8} \approx 4.25 \times 10^{14}$$

> **Interpretación:** La aceleración centrípeta es ~425 billones de veces la gravedad terrestre. Esta aceleración enorme es proporcionada por la fuerza que mantiene al electrón en trayectoria circular (en el contexto físico real, la fuerza de Lorentz, pero aquí solo la cuantificamos cinemáticamente).

**(e) Vueltas en 1 microsegundo ($\Delta t = 10^{-6}$ s):**
$$N = \frac{\Delta t}{T} = \frac{10^{-6}}{3.77 \times 10^{-8}} \approx 26.53 \text{ vueltas}$$

> **Verificación:** $N = f \times \Delta t = 26.53 \times 10^6 \times 10^{-6} = 26.53$ vueltas. Consistente.

**(f) Distancia total recorrida:**
$$s = v \times \Delta t = 2.5 \times 10^7 \times 10^{-6} = 25 \text{ m}$$

> **Verificación alternativa:** $s = N \times (2\pi R) = 26.53 \times 2\pi \times 0.15 = 26.53 \times 0.9425 \approx 25$ m. Consistente.

**3. Discusión Crítica:**
* **Movimiento "uniforme" vs. "acelerado":** Aunque la rapidez es constante, el movimiento está acelerado porque la dirección de $\vec{v}$ cambia continuamente. La aceleración $\vec{a}_c$ siempre apunta al centro, siendo perpendicular a $\vec{v}$.
* **Validez del modelo circular:** En una cámara de burbujas real, la trayectoria es una espiral hacia adentro porque el electrón pierde energía por ionización del medio. El MCU es una aproximación válida para tramos cortos donde la pérdida de energía es despreciable.
* **Límite de velocidad:** A $v = 2.5 \times 10^7$ m/s (~8% de la velocidad de la luz), los efectos relativistas son pequeños pero medibles. La masa del electrón aumenta un ~0.3%, lo que modificaría ligeramente el radio si la fuerza centrípeta fuera constante.

**4. Análisis de Sensibilidad:**
- **La aceleración centrípeta** es extremadamente sensible a cambios en velocidad (cuadrática), un aumento en el 10% de la velocidad la aceleración centrìpeta aumenta en un 21%.

**5. Extensión:**
* **Aplicación en detectores:** Los físicos de partículas usan la curvatura de trayectorias en campos magnéticos para identificar partículas. Partículas con igual velocidad pero diferente masa describen radios diferentes.

* **Espectrómetros de masa:** En un espectrómetro de masa, todos los iones son acelerados y disparados hacia el interior de un cámara con campo magnético uniforme, cada ion describe una trayectoria semi círcular cuyo radio esta en función de la masa del ion.

```
---

## 📓 III. Actividades para el Portafolio Digital

Resuelve los siguientes desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.

---

### 🧠 Desafío 1

**El Barco Patrullero en el Estrecho**

Un barco patrullero debe cruzar un estrecho de ancho $D = 2$ km. Su motor le permite una rapidez $v_b = 15$ km/h en aguas tranquilas. La corriente del estrecho tiene una rapidez $v_c = 5$ km/h.

* **El Reto:** Calcula el ángulo respecto a la perpendicular que debe mantener el timonel para llegar exactamente al puerto frente al punto de partida, y el tiempo de cruce.
* **Interpretación:** ¿Por qué en navegación marítima este cálculo es crítico para evitar arenas movedizas en las orillas?
* **Simulación GeoGebra:** Ajusta los vectores velocidad y observa la trayectoria resultante.

---

### 🧠 Desafío 2
**El Lanzamiento del Rescate Aéreo**

Un helicóptero de rescate vuela horizontalmente a $v = 90$ km/h a una altura $h = 80$ m sobre el nivel del mar. Debe lanzar una cápsula de rescate a un bote en el agua.

* **El Reto:** Determina la distancia horizontal desde el bote a la cual debe soltarse la cápsula, y la velocidad de impacto con el agua.
* **Análisis Crítico:** Si el viento genera una deriva horizontal adicional de $v_v = 10$ m/s, ¿cómo afecta esto al punto de impacto? ¿Debe el helicóptero compensar antes de soltar?
* **Simulación GeoGebra:** Varía la altura y velocidad inicial.

---

### 🧠 Desafío 3
**El Cañón de Festejos**

Un cañón de feria dispara proyectiles con $v_0 = 25$ m/s. El blanco está colocado en una plataforma a $h = 5$ m de altura y a una distancia horizontal $d = 30$ m.

* **El Reto:** Determina los dos ángulos de disparo posibles para impactar el blanco y el tiempo de vuelo para cada trayectoria.
* **Toma de Decisión:** ¿Cuál ángulo es preferible si detrás del blanco hay una multitud a $40$ m? Justifica tu respuesta con el análisis de la parábola de seguridad.
* **Simulación GeoGebra:** Ajusta el ángulo para alcanzar el blanco.

---

### 🧠 Desafío 4
**El Esquiador en la Rampa**

Un esquiador salta desde una rampa inclinada $\alpha = 30°$ respecto a la horizontal con velocidad $v_0 = 12$ m/s. La rampa termina en un declive con el mismo ángulo $\alpha$.

* **El Reto:** Calcula la distancia máxima alcanzada medida a lo largo del declive (alcance en plano inclinado) y el tiempo de vuelo.
* **Análisis Técnico:** ¿Cuál sería el ángulo óptimo de salto (respecto a la horizontal) para maximizar el alcance sobre el declive? Compara con el resultado teórico $\theta_{opt} = 45° - \frac{\alpha}{2}$.
* **Simulación GeoGebra:** Visualiza la trayectoria sobre la pendiente.

---

### 🧠 Desafío 5
**El Ciclotrón de Partículas**

En un ciclotrón, un protón describe una trayectoria circular de radio variable. Inicialmente gira con velocidad angular constante $\omega_0 = 5 \times 10^6$ rad/s en una órbita de radio $R_0 = 10$ cm.

* **El Reto:** Calcula la rapidez lineal del protón, su período de revolución y la aceleración centrípeta en la órbita inicial. Si el radio se expande uniformemente a razón de $2$ cm por microsegundo mientras $\omega$ se mantiene constante, ¿cuál es la rapidez del protón después de $3$ microsegundos?
* **Interpretación Profesional:** ¿Por qué en ciclotrones reales la frecuencia de rotación debe ajustarse cuando el radio cambia? Relaciona con la condición de sincronización entre la frecuencia del campo oscilante y la frecuencia de revolución de la partícula.
* **Simulación GeoGebra:** Observa cómo cambian $v$ y $a_c$ al modificar el radio.

---

### 🧠 Desafío 6
**La Centrifugadora de Laboratorio**

Un rotor de centrifugadora de radio $R = 15$ cm acelera desde el reposo con aceleración angular constante $\alpha = 500$ rad/s² durante $10$ s, luego mantiene velocidad angular constante por $30$ s, y finalmente frena con $\alpha = -1000$ rad/s² hasta detenerse.

* **El Reto:** Grafica $\omega(t)$, $a_t(t)$ y $a_c(t)$ en función del tiempo. Calcula la aceleración total máxima y en qué instante ocurre. ¿Cuántas revoluciones completas da el rotor durante todo el ciclo?
* **Análisis de Sensibilidad:** Si la muestra contiene células que se dañan con aceleraciones centrípetas superiores a $3000g$, ¿es seguro usar esta centrifugadora? ¿En qué fase del ciclo está el mayor riesgo?
* **Simulación GeoGebra:** Observa la variación de las componentes de aceleración.

---

### 🧠 Desafío 7
**El Satélite en Órbita Baja**

Un satélite describe una órbita circular a una altura donde el radio orbital total es $R = 6771$ km. Su período orbital medido es $T = 5550$ s.

* **El Reto:** Calcula la velocidad angular, la rapidez lineal orbital y la aceleración centrípeta del satélite. Si el satélite reduce su velocidad un 1% manteniendo la dirección tangencial, ¿cuál sería el radio de curvatura de su nueva trayectoria en ese instante?
* **Análisis Crítico:** ¿Es posible que el satélite mantenga una órbita circular con velocidad diferente a la calculada manteniendo el mismo radio? Justifica cinemáticamente tu respuesta usando la relación entre $v$, $\omega$ y $R$.
* **Simulación GeoGebra:** Ajusta el radio y observa los cambios en velocidad y período.

---

### 🧠 Desafío 8
**La Bola de Demolición**

Una bola de demolición cuelga de un cable de longitud $L = 12$ m. Un operador la impulsa horizontalmente desde el reposo con velocidad inicial $v_0 = 4$ m/s perpendicular al cable, describiendo desde ese instante un arco circular.

* **El Reto:** Calcula la rapidez angular inicial de la bola, la aceleración centrípeta en el punto de lanzamiento y el período de revolución si mantuviera velocidad angular constante. Si el cable se corta exactamente a los $2$ segundos de iniciado el movimiento, calcula la posición angular alcanzada hasta ese instante y describe la trayectoria subsiguiente (radio de curvatura en el instante del corte y dirección inicial de la velocidad).
* **Interpretación Técnica:** ¿Por qué los operadores de grúas deben controlar la rapidez inicial de impulso? Relaciona con la aceleración centrípeta instantánea que aparece al pasar del reposo al movimiento circular ($a_c = v_0^2/L$).
* **Simulación GeoGebra:** Observa la transición entre trayectoria circular y línea recta tangente.

---

### 🧠 Desafío 9
**El Tubo de Rayos Catódicos (CRT)**

En un osciloscopio, un electrón entra a una región de placas deflectoras con velocidad horizontal constante $v_x = 3 \times 10^7$ m/s. Dentro de las placas de longitud $L = 4$ cm, adquiere una aceleración vertical constante $a_y = 8.8 \times 10^{14}$ m/s².

* **El Reto:** Calcula el tiempo que el electrón permanece dentro de las placas, la deflexión vertical al salir y el ángulo de salida respecto a la horizontal. Si la pantalla está a $D = 20$ cm de las placas, ¿dónde impacta el electrón medido desde el eje central?
* **Evaluación:** ¿Es válido despreciar la aceleración gravitatoria ($g = 9.8$ m/s²) en este cálculo? Compara órdenes de magnitud entre $a_y$ y $g$ para justificar.
* **Simulación GeoGebra:** Modela la trayectoria parabólica con aceleración constante vertical.

---

### 🧠 Desafío 10
**La Cinta Transportadora Curva**

Una cinta transportadora curva de radio $R = 2$ m mueve cajas con rapidez constante $v = 1.5$ m/s. El diseñador sabe que para mantener el movimiento circular se requiere una aceleración centrípeta $a_c = v^2/R$.

* **El Reto:** Calcula la aceleración centrípeta requerida y determina qué sucede si la cinta aumenta su rapidez a $v = 3$ m/s manteniendo el mismo radio (¿cuánto aumenta $a_c$?). Si el ingeniero necesita duplicar el caudal de transporte, compara cinemáticamente tres alternativas: (A) duplicar la velocidad a $v = 3$ m/s con $R = 2$ m, (B) instalar una segunda cinta idéntica en paralelo con $v = 1.5$ m/s, o (C) aumentar el radio a $R = 4$ m manteniendo $v = 1.5$ m/s. ¿Cuál alternativa genera menor aceleración centrípeta por caja?
* **Toma de Decisión:** Una caja puede soportar aceleraciones centrípetas hasta $a_{max} = 5$ m/s² sin dañarse. ¿Cuál es la rapidez máxima permitida en la curva de $R = 2$ m? ¿Y si se amplía a $R = 4$ m? Presenta una tabla comparativa de velocidades máximas según el radio.
* **Simulación GeoGebra:** Observa cómo varía $a_c$ al modificar $v$ y $R$ con deslizadores.

