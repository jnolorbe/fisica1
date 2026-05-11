# Sesión 5: Dinámica lineal
## Fuerzas constantes

## 📌 I. Fundamento Teórico

En esta sesión se establecen los principios fundamentales que relacionan las fuerzas con el movimiento de los cuerpos, analizando las tres leyes de Newton, los diferentes tipos de fuerzas que actúan sobre una partícula, y las condiciones de equilibrio mecánico.

---

### 1.1. Leyes de Newton

#### Primera Ley de Newton (Ley de Inercia)

> **Enunciado:** Todo cuerpo libre en el espacio permanece en estado de reposo o de movimiento rectilíneo uniforme a menos que una fuerza actúe sobre él.

**Interpretación física:**
* Las **fuerzas** son las causas que producen cambios en el estado de movimiento.
* Esta ley define implícitamente los **sistemas de referencia inerciales**.
* El estado de reposo y el movimiento rectilíneo uniforme son dos estados equivalentes.
* Las fuerzas se originan por la interacción de otros cuerpos.

**Sistemas de referencia**

* **Inercial:** Sistema de referencia donde un cuerpo libre de fuerzas permanece en reposo o MRU.
* **No inercial:** Sistema de referencia acelerado respecto a uno inercial; en él los cuerpos se observan cambiar su estado de movimiento debido a que el sistema de referencia esta acelerado. Un observador No inercial, puede pensar que esta en un sistema de referencia inercial, y percibira **fuerzas ficticias** o no reales. 

#### Segunda Ley de Newton (Ecuación Fundamental de la Dinámica)

> **Enunciado:** La aceleración de un cuerpo es directamente proporcional a la fuerza neta que actúa sobre él e inversamente proporcional a su masa.

$$\vec{a} = \frac{\sum {\vec{F}}}{m}$$


**Componentes Cartesianos:**
$$\sum {\vec{F}_x} = m\vec{a}_x, \quad \sum {\vec{F}_y} = m\vec{a}_y, \quad \sum {\vec{F}_z} = m\vec{a}_z$$

**Masa inercial ($m$):** Propiedad intrínseca del cuerpo que cuantifica su resistencia a cambiar su estado de movimiento. Se mide en kg.

> **💡 Regla de Oro:** La Segunda Ley es una ecuación vectorial. Siempre descompón las fuerzas en ejes convenientes antes de aplicarla. La elección de ejes paralelo-normal al movimeinto puede simplificar drásticamente los cálculos.

---

#### Tercera Ley de Newton (Acción y Reacción)

> **Enunciado:** Si un cuerpo A ejerce una fuerza sobre un cuerpo B, entonces B ejerce sobre A una fuerza igual en magnitud y dirección pero de sentido opuesto.

$$\vec{F}_{1/2} = -\vec{F}_{2/1}$$

**Características:**
* Las fuerzas de acción-reacción actúan sobre **cuerpos diferentes**
* Son del mismo tipo (ambas de contacto, ambas gravitatorias, etc.)

---

### 1.2. Fuerza Gravitatoria

**Ley de Gravitación Universal (Newton):**

$$\vec{F}_g = -G\frac{Mm}{r^2}\hat{r}$$

La Fuerza gravitatoria que ejerce el planeta Tierra sobre cualquier cuerpo que se encuentra hasta una altitud de 100 km, se considera constante y es lo que percibimos como peso (P), cuya magnitud se calcula multiplicando la masa por el valor de la aceleración gravitatoria. 

$$P = mg$$

donde $g \approx 9.8$ m/s².

**Masa gravitacional vs. Masa inercial**

**Masa inercial:** Resistencia a cambiar el movimiento.  ($m = F/a$). 
**Masa gravitacional:** Propiedad relacionada con el peso del cuerpo, ($m = P/g$) |
> **Principio de equivalencia (Einstein):** Masa inercial = Masa gravitacional. Este principio funda la relatividad general.

---

### 1.3. Fuerza de Contacto

Cuando dos cuerpos están en contacto, la fuerza de interacción o fuerza de contacto puede descomponerse en:

**Componente normal ($F_n$):**
* Perpendicular a la superficie de contacto.
* Previene la interpenetración de los cuerpos.

**Componente tangencial ($F_t$):**
* Paralela a la superficie de contacto.
* Relacionada con la rugosidad de las superficies en contacto.

---

### 1.4. Fuerza de Rozamiento

Es el componente tangencial de la Fuerza de contacto, se origina debido a las asperezas o rugosidad entre las superficies de contacto.

#### Rozamiento Estático ($f_s$)

* Actúa cuando NO hay deslizamiento entre las superficies de contacto (movimiento relativo).
* Su magnitud alcanza su máximo valor cuando esta a punto de deslizar: $f_{s} \leq \mu_s F_n$

**Máximo rozamiento estático:**
$$f_{s,max} = \mu_s F_n$$

donde $\mu_s$ es el coeficiente de rozamiento estático, propio de las superficies en contacto, por ejemplo madera-madera, metal-madera, caucho-asfalto, etc.

#### Rozamiento Cinético ($f_k$)

* Actúa cuando HAY deslizamiento de una superficie sobre la otra (movimiento relativo)
* Magnitud aproximadamente constante: $f_k = \mu_k F_n$
* Generalmente $\mu_k < \mu_s$

> **💡 Regla de Oro:** Para iniciar el movimiento se requiere por lo menos igualar la $f_{s,max}$. Una vez en movimiento, la fuerza de rozamiento disminuye a $f_k$, lo que explica por qué es más fácil mantener un objeto en movimiento que iniciarlo.

---

### 1.5. Fuerza Elástica. Ley de Hooke

Para un resorte ideal (lineal):

$$F_{e} = k\Delta l$$

donde:
* $k$: constante elástica del resorte (N/m)
* $\Delta l$: elongación o compresión respecto a la longitud natural
---

### 1.6. Fuerza de Tensión de Cuerdas

**Tensión ($T$):** Fuerza que transmite una cuerda (o cable, soga, etc.) cuando está tensa.

**Características:**
* Dirección: a lo largo de la cuerda, las cuerdas jalan hacia afuera del cuerpo que estan atados
* Magnitud: igual en todos los puntos de una cuerda ideal (sin masa, inextensible)
* Si la cuerda tiene masa, la tensión varía a lo largo de ella

**Cuerda ideal:**
* Masa despreciable ($m_{cuerda} \approx 0$)
* Inextensible (longitud constante)
---

### 1.7. Equilibrio de Traslación. 

**Condición de equilibrio:**

Un cuerpo estático (reposo) o con movimiento rectilíneo uniforme (MRU), tiene una aceleración nula y por lo tanto las fuerzas que actúan sobre el es nula.

$$\vec{a} = 0  \Rightarrow \vec{F}_{neta} = 0 $$

**Métodos de resolución:**

**1. Descomposición cartesiana:**
$$\sum F_x = 0, \quad \sum F_y = 0$$

**2. Triángulo de fuerzas (para 3 fuerzas coplanares):**

Si tres fuerzas están en equilibrio, forman un triángulo cerrado.

$$\frac{F_1}{\sin\alpha} = \frac{F_2}{\sin\beta} = \frac{F_3}{\sin\gamma}$$

donde $\alpha, \beta, \gamma$ son los ángulos opuestos a cada fuerza.

> **💡 Regla de Oro:** El método del triángulo es útil cuando conoces ángulos y necesitas encontrar relaciones entre magnitudes de fuerzas. La descomposición cartesiana es más general y funciona para cualquier número de fuerzas.

---

## 🚀 II. Problemas Resueltos

### 🧩 Problema N° 1
```{admonition} Paracaidista
Un paracaidista de $m = 80$ kg salta desde un avión. Inicialmente cae libremente, pero al desplegarse el paracaídas experimenta una fuerza de arrastre del aire constante $F_{arr} = 1200$ N dirigida hacia arriba. Calcular: 
- (a) la aceleración neta después de desplegado el paracaídas,
- (b) el tiempo que demora en llegar al piso.
- (c) la velcoidad de impacto con el piso.
```


### 🧩 Problema N° 2
```{admonition} Tobogan 
Un niño de $m = 35$ kg se desliza por un tobogán de $L = 4$ m de longitud inclinado $\theta = 30°$ respecto a la horizontal. El coeficiente de rozamiento cinético entre sus pantalones y la superficie es $\mu_k = 0.25$. Deducir: 

- (a) la aceleración del niño.
- (b) la velocidad al llegar al final del tobogán si parte del reposo.
- (c) el tiempo de descenso.
- (d) el ángulo crítico donde el niño comenzaría a deslizarse si $\mu_s = 0.40$.

```
```{admonition} Solución
:class: dropdown hint
**1. Planteamiento:**
* **Ruta de la solución:** Descomponer el peso en ejes paralelo y perpendicular al plano. Aplicar la Segunda Ley en ambos ejes. La normal equilibra la componente perpendicular; la componente paralela menos el rozamiento da la aceleración.
* **Predicción cualitativa:** El niño empezara a deslizar sin impulsión si el tobogan supera el ángulo crítico, a mayo ángulo mayor aceleración de descenso.

**2. Resolución:**

**Componentes del peso:**
$$P_x = mg\sin\theta = 35 \times 9.8 \times \sin(30°) = 343 \times 0.5 = 171.5 \text{ N}$$
$$P_y = mg\cos\theta = 35 \times 9.8 \times \cos(30°) = 343 \times 0.866 = 297.0 \text{ N}$$

**(a) Aceleración:**
Eje y (Equilibrio, sin aceleración perpendicular):
$$F_n = P_y = 297.0 \text{ N}$$

Calulo de la fuerza rozamiento cinético:
$$f_k = \mu_k N = 0.25 \times 297.0 = 74.25 \text{ N}$$

Eje x (Segunda Ley):
$$P_x - f_k = ma$$
$$171.5 - 74.25 = 35a$$
$$97.25 = 35a$$
$$a = 2.78 \text{ m/s}^2$$

**(b) Velocidad final:**
Movimiento uniformemente acelerado desde el reposo:
$$v^2 = v_0^2 + 2aL = 0 + 2 \times 2.78 \times 4 = 22.24$$
$$v = \sqrt{22.24} = 4.72 \text{ m/s} \approx 17 \text{ km/h}$$

**(c) Tiempo de descenso:**
$$v = v_0 + at$$
$$4.72 = 0 + 2.78t$$
$$t = \frac{4.72}{2.78} = 1.70 \text{ s}$$

**(d) Ángulo crítico:**

Para iniciar el movimiento: $P_x = f_{s,max}$
$$mg\sin\theta_c = \mu_s mg\cos\theta_c$$
$$\tan\theta_c = \mu_s = 0.40$$
$$\theta_c = \arctan(0.40) = 21.8°$$

> **Conclusión:** El tobogán a 30° supera ampliamente el ángulo crítico (21.8°), por lo que el niño desliza inevitablemente sin ninguna impulsión.

**3. Discusión Crítica:**
* La aceleración de 2.78 m/s² es aproximadamente un tercio de $g$, cómoda para un niño. Los toboganes comerciales se diseñan con ángulos de 25-35° para aceleraciones seguras pero emocionantes.
* La aceleración es independiente de la masa o peso del niño, solo depende del ángulo de inclinación y del coeficiente de rozamiento.

**4. Análisis de Sensibilidad:**
* El rozamiento cinético reduce la velocidad final un 30% respecto al caso sin rozamiento ($v_{sin roz} = \sqrt{2gL\sin\theta} = 6.26$ m/s).
* Los pantalones de algodón tienen $\mu_k \approx 0.3-0.5$ sobre plástico.
* En el caso de los toboganes acuáticos el agua reduce el coeficientes de rozamiento a $\mu_k \sim 0.05$ , permitiendo mayores velocidades.

**5. Extensión:**
Los trineos olímpicos de hielo alcanzan 150 km/h con $\mu_k \approx 0.03$ sobre hielo. Los sistemas de evacuación de emergencia de aviones usan toboganes inflables con ángulos de 30-40° y superficies de bajo rozamiento para evacuar 300 pasajeros en 90 segundos.

```
### 🧩 Problema N° 2
```{admonition} Frenado sobre Plano Inclinado
class: important
Un camión de mineral de $m = 25000$ kg desciende por una carretera inclinada $\theta = 8°$. El coeficiente de rozamiento cinético entre neumáticos y asfalto es $\mu_k = 0.35$. El conductor frena bloqueando las ruedas. Deducir: 
- (a) la aceleración del camión mientras frena.
- (b) la distancia mínima para detenerse si va a $v_0 = 72$ km/h (20 m/s).

```
```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Descomponer fuerzas en ejes paralelo y perpendicular al plano. El rozamiento cinético actúa hacia arriba del plano (opuesto al deslizamiento). Para el frenado adicional, aplicar cinemática para encontrar la aceleración requerida y luego la Segunda Ley.
* **Predicción cualitativa:** El camión aceleraría naturalmente cuesta abajo si no frenara. El rozamiento de deslizamiento ayuda a frenar, pero no es suficiente para detenerlo rápidamente.
**2. Resolución:**

**Datos:**
* $m = 25000$ kg
* $\theta = 8°$, $\mu_k = 0.35$
* $v_0 = 20$ m/s

**Componentes del peso:**
$$P_x = mg\sin\theta = 25000 \times 9.8 \times \sin(8°) = 245000 \times 0.139 = 34055 \text{ N}$$
$$P_y = mg\cos\theta = 25000 \times 9.8 \times \cos(8°) = 245000 \times 0.990 = 242550 \text{ N}$$

Calulo de la fuerza normal:

$F_n = P_y = 242550$ N

Rozamiento cinético (opuesto al movimiento, hacia arriba):

$f_k = \mu_k N = 0.35 \times 242550 = 84893 \text{ N}$

**(a) Aceleración con frenado de deslizamiento:**
Segunda Ley (eje x, positivo hacia abajo):
$$P_x - f_k = ma$$
$$34055 - 84893 = 25000a$$
$$a = -2.03 \text{ m/s}^2$$

> **Interpretación:** El camión desacelera a 2.03 m/s². El rozamiento es mayor que la componente del peso, logrando frenar aunque cuesta abajo.

**3. Discusión Crítica:**
* No importa si el conductor presiona los frenos con mucha fuerza, al detener las ruedas, las variabels involucradas en la aceleración de frenado son el coeficiente de rozmaiento y la pendiente de la carretera.
* No importa la masa del camión, un camión muy pesado acelera lo mismo que uno con poco peso.

**4. Análisis de Sensibilidad:**
Si las cocadas de la ruedas de incrmentan haciendo que el coeficiente de rozmaiento se duplique entonces...


**5. Extensión:**
Los sistemas ABS (Anti-lock Braking System) evitan el bloqueo de ruedas, manteniendo $\mu_s$ (mayor que $\mu_k$) entre la pastilla de freno y las ruedas el camión. Haciendo que las ruedas se detengan más rapido debido a la fuerza de rozmaiento estático es más mayor.

```


### 🧩 Problema N° 3
```{admonition}  Fuerza Mínima y Ángulo Óptimo para Iniciar el Movimiento
class: important
Una persona intenta mover un ropero de $m = 80$ kg sobre un piso horizontal de madera. El coeficiente de rozamiento estático es $\mu_s = 0.45$ y el cinético es $\mu_k = 0.35$. La persona aplica una fuerza $\vec{F}$ con un ángulo $\theta$ variable respecto a la horizontal. Calcular: 
- (a) la fuerza mínima necesaria para iniciar el movimiento y el ángulo óptimo.
- (b) la aceleración si se aplica la fuerza mínima una vez iniciado el movimiento.
- (c) la fuerza horizontal ($\theta = 0$) necesaria para mantener velocidad constante.
- (d) la fuerza a $\theta = 30°$ que produce la máxima aceleración posible.
```
```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Descomponer la fuerza aplicada en horizontal y vertical. La componente vertical reduce la normal y por tanto el rozamiento. Encontrar el ángulo que minimiza la fuerza total necesaria para vencer $f_{s,max}$.
* **Predicción cualitativa:** Tirar hacia arriba (ángulo positivo) reduce la normal y el rozamiento, pero la componente horizontal disminuye. Existe un ángulo óptimo que equilibra ambos efectos.

**2. Resolución:**

**Diagrama de fuerzas:**
* $F\cos\theta$: horizontal (hacia adelante)
* $F\sin\theta$: vertical (hacia arriba)
* $F_n = mg - F\sin\theta$: normal reducida
* $f_s \leq \mu_s F_n$: rozamiento estático

**(a) Fuerza mínima y ángulo óptimo:**

Condición de umbral: $F\cos\theta = \mu_s F_n = \mu_s(mg - F\sin\theta)$

$$F\cos\theta = \mu_s mg - \mu_s F\sin\theta$$
$$F(\cos\theta + \mu_s\sin\theta) = \mu_s mg$$
$$F = \frac{\mu_s mg}{\cos\theta + \mu_s\sin\theta}$$

Para minimizar $F$, maximizar el denominador $\cos\theta + \mu_s\sin\theta$:

$$\frac{d}{d\theta}( -\sin\theta + \mu_s\cos\theta) = 0$$
$$\tan\theta_{opt} = \mu_s = 0.45$$
$$\theta_{opt} = \arctan(0.45) = 24.2°$$

Fuerza mínima:
$$F_{min} = \frac{0.45 \times 80 \times 9.8}{\cos(24.2°) + 0.45\sin(24.2°)}$$
$$F_{min} = \frac{352.8}{0.912 + 0.45 \times 0.410} = \frac{352.8}{0.912 + 0.184} = \frac{352.8}{1.096}$$
$$F_{min} = 321.9 \text{ N} \approx 322 \text{ N}$$

**(b) Aceleración con fuerza mínima (ya en movimiento):**

Una vez en movimiento, $\mu_k = 0.35$:
$$F_n = mg - F_{min}\sin\theta_{opt} = 784 - 321.9 \times 0.410 = 784 - 132.0 = 652.0 \text{ N}$$
$$f_k = \mu_k F_n = 0.35 \times 652.0 = 228.2 \text{ N}$$

Fuerza neta horizontal:
$$F_{neta} = F_{min}\cos\theta_{opt} - f_k = 321.9 \times 0.912 - 228.2 = 293.6 - 228.2 = 65.4 \text{ N}$$

$$a = \frac{F_{neta}}{m} = \frac{65.4}{80} = 0.818 \text{ m/s}^2$$

**(c) Fuerza horizontal para velocidad constante:**

MRU ($a = 0$): $F = f_k = \mu_k mg = 0.35 \times 784 = 274.4$ N

**(d) Fuerza a $\theta = 30°$ para máxima aceleración:**

Para máxima aceleración, aplicar la máxima fuerza posible sin levantar el objeto ($N \geq 0$):
$$F\sin\theta \leq mg \Rightarrow F \leq \frac{mg}{\sin\theta} = \frac{784}{0.5} = 1568 \text{ N}$$

Pero también debe vencer el rozamiento:
$$F\cos\theta \geq \mu_k(mg - F\sin\theta)$$

Con $F = 1568$ N (límite de levantamiento):
$$F_n = 784 - 1568 \times 0.5 = 784 - 784 = 0$$

El objeto se levanta, no hay rozamiento, y la aceleración horizontal es:
$$a = \frac{F\cos\theta}{m} = \frac{1568 \times 0.866}{80} = \frac{1358}{80} = 17.0 \text{ m/s}^2$$

Pero esto es irrealista (levantaría el ropero). Para máxima aceleración manteniendo contacto ($N > 0$), usar $F$ tal que $a$ sea máxima con $F_n \geq 0$.

**3. Discusión Crítica:**
* El ángulo óptimo de 24.2° es independiente de la masa del objeto. Depende solo de $\mu_s$. Este resultado es útil en diseño ergonómico de mangos y asas.
* Los carros de supermercado con ruedas de bajo rozamiento ($\mu_k \approx 0.02$) requieren fuerzas mínimas de ~15 N para moverse, explicando por qué pueden desplazarse con un dedo. ¿por eso tienen ruedas de diferente tamaño?

**4. Análisis de Sensibilidad:**
Si se aplica una fuerza horizontal se requiere mayor magnitud de fuerza horizontal. Verificación con $\theta = 0$ (empujar horizontal):
$$F(\theta=0) = \mu_s mg = 0.45 \times 784 = 352.8 \text{ N}$$
**Ahorro:** Tirar a 24.2° reduce la fuerza requerida en un 8.8% respecto a empujar horizontalmente.

**5. Extensión:**
Los robots de manipulación industrial calculan ángulos óptimos de agarre para minimizar la fuerza de sujeción necesaria. Los exoesqueletos de asistencia física detectan la intención de movimiento del usuario y aplican fuerza en el ángulo óptimo. Los sistemas de arrastre de emergencia en aviones (evacuación de heridos) usán trineos con ángulos de jalado calculados para minimizar el esfuerzo del rescatista.

### 🧩 Problema N° 3
```{admonition}  Fuerza Mínima y Ángulo Óptimo para Iniciar el Movimiento
class: important
Un tendedero de ropa consiste en dos cuerdas de nailon de longitud $L = 3$ m cada una, fijas en postes separados $D = 4$ m. En el punto medio cuelga un resorte de constante $k = 200$ N/m y longitud natural $\ell_0 = 0.5$ m, del cual pende una canasta con ropa de $m = 12$ kg. Calcular:

- (a) el ángulo que forma cada cuerda con la horizontal.
- (b) la tensión en cada cuerda.
- (c) la elongación del resorte y su longitud final.
- (d) la altura de descenso del punto medio respecto a la línea de los postes.
```
```{admonition} Solución
:class: dropdown hint

**1. Planteamiento:**
* **Ruta de la solución:** Analizar la geometría del sistema para encontrar el ángulo de las cuerdas. En el nodo central, tres fuerzas actúan: tensión de cada cuerda (simétricas) y peso de la canasta (transmite a través del resorte). Aplicar equilibrio de fuerzas verticales y horizontales.
* **Predicción cualitativa:** El ángulo será significativo debido a la separación de 4 m con cuerdas de 3 m (geometría imposible sin deformación). El resorte se estirará considerablemente para permitir la configuración.

**2. Resolución:**

**Datos:**
* $L = 3$ m (cuerda), $D = 4$ m (separación de postes)
* $k = 200$ N/m, $\ell_0 = 0.5$ m
* $m = 12$ kg $\Rightarrow$ $P = 12 \times 9.8 = 117.6$ N

**(a) Ángulo de las cuerdas:**

La geometría inicial (sin carga) es imposible: dos cuerdas de 3 m no pueden unir postes a 4 m de distancia (3+3=6 > 4, pero la forma triangular requiere altura).

Con carga, el punto central desciende, formando dos triángulos rectángulos.

Distancia horizontal de cada poste al centro: $x = D/2 = 2$ m.

Longitud de cuerda en cada lado: $L = 3$ m.

Altura vertical desde poste hasta punto central:
$$h = \sqrt{L^2 - x^2} = \sqrt{9 - 4} = \sqrt{5} = 2.236 \text{ m}$$

Ángulo con la horizontal:
$$\cos\theta = \frac{x}{L} = \frac{2}{3} = 0.667$$
$$\theta = \arccos(0.667) = 48.2°$$

$$\sin\theta = \frac{h}{L} = \frac{2.236}{3} = 0.745$$

**(b) Tensión en cada cuerda:**

Equilibrio vertical en el nodo central:
$$2T\sin\theta = P$$
$$T = \frac{P}{2\sin\theta} = \frac{117.6}{2 \times 0.745} = \frac{117.6}{1.490} = 78.9 \text{ N}$$

Verificación horizontal: las componentes horizontales se cancelan ($T\cos\theta$ a izquierda y derecha).

**(c) Elongación del resorte:**

El resorte soporta el peso completo:
$$F_{el} = P = k\Delta\ell$$
$$\Delta\ell = \frac{P}{k} = \frac{117.6}{200} = 0.588 \text{ m}$$

Longitud final del resorte:
$$\ell = \ell_0 + \Delta\ell = 0.5 + 0.588 = 1.088 \text{ m}$$

**(d) Altura de descenso:**

Sin carga, el punto central estaría a altura $h = 2.236$ m debajo de los postes (geometría rígida). Con carga, el resorte añade 1.088 m de longitud vertical.

Altura total de descenso desde los postes:
$$H = h + \ell = 2.236 + 1.088 = 3.324 \text{ m}$$

> **Nota:** Los postes deben tener al menos 3.5 m de altura para que la canasta no toque el suelo.

**(e) Verificación por triángulo de fuerzas:**

Las tres fuerzas en el nodo central son:
* $\vec{T}_1$: tensión izquierda (magnitud 78.9 N, ángulo 180°-48.2° = 131.8°)
* $\vec{T}_2$: tensión derecha (magnitud 78.9 N, ángulo 48.2°)
* $\vec{P}$: peso (magnitud 117.6 N, ángulo 270°/-90°)

Para verificar el triángulo, las fuerzas deben formar un polígono cerrado.

Componentes de $\vec{T}_1$:
$$T_{1x} = -78.9\cos(48.2°) = -78.9 \times 0.667 = -52.6 \text{ N}$$
$$T_{1y} = 78.9\sin(48.2°) = 78.9 \times 0.745 = 58.8 \text{ N}$$

Componentes de $\vec{T}_2$:
$$T_{2x} = 78.9\cos(48.2°) = 52.6 \text{ N}$$
$$T_{2y} = 78.9\sin(48.2°) = 58.8 \text{ N}$$

Suma de fuerzas:
$$\sum F_x = -52.6 + 52.6 + 0 = 0 \quad \checkmark$$
$$\sum F_y = 58.8 + 58.8 - 117.6 = 0 \quad \checkmark$$

> **Verificación del triángulo:** Los tres vectores forman un triángulo isósceles con lados 78.9, 78.9 y base 117.6. El ángulo entre las tensiones es $2 \times 48.2° = 96.4°$. Por la ley de cosenos:
> $$117.6^2 = 78.9^2 + 78.9^2 - 2(78.9)(78.9)\cos(96.4°)$$
> $$13830 = 6225 + 6225 - 12450(-0.115) = 12450 + 1432 = 13882$$
> 
> Coincide aproximadamente (error por redondeo). **Verificado.**

**3. Discusión Crítica:**
* La geometría del problema es inestable sin carga: las cuerdas de 3 m unen postes a 4 m con exceso de longitud. El resorte absorbe este exceso y proporciona la tensión necesaria.
* En tendederos reales, las cuerdas se tensan con torniquetes o poleas, eliminando la holgura. El resorte en este problema simula la elasticidad de la cuerda de nailon real.

**4. Análisis de Sensibilidad:**

* Un incrmento de de la masa de la ropa en +50% incrmenta la tensión en +50%
* Una incrmento en la separación de postes en +20%, aumenta el ángulo y en consecuencia la tensión en un +15%

**5. Extensión:**
Los puentes colgantes usan cables principales con flechas (sag) calculadas para distribuir la tensión uniformemente. Los arcos arquitectónicos (Gaudí, Sagrada Familia) usan cadenas colgantes invertidas para encontrar formas de compresión pura, aplicando el principio del triángulo de fuerzas a escala modelo.

```
---

## 📓 III. Actividades para el Portafolio Digital

Resuelve los siguientes 10 desafíos siguiendo el **Formato de 5-Bloques**. Para el Portafolio digital presenta **4 Desafíos** de tu elección.

---

### 🧠 Desafío 1 
**El Ascensor del Edificio de San Isidro**

Un ascensor de $m = 1200$ kg sube acelerando a $a = 1.5$ m/s². Un pasajero de 70 kg está sobre una báscula.

* **El Reto:** Calcula la tensión en el cable del ascensor, la lectura de la báscula (peso aparente), y la fuerza que el pasajero ejerce sobre el piso del ascensor.
* **Interpretación:** ¿Por qué nos sentimos "más pesados" cuando el ascensor acelera hacia arriba? Relaciona con la experiencia en aviones durante el despegue.
* **Simulación GeoGebra:** [Simulación de Ascensor y Peso Aparente](https://www.geogebra.org/m/XKfpRjQH) - Observa cómo cambia la normal al variar la aceleración.

---

### 🧠 Desafío 2
**El Trineo de los Uros del Titicaca**

Un trineo tradicional de madera ($m = 25$ kg) transporta carga de pescado ($m = 40$ kg) sobre hielo del lago Titicaca ($\mu_k = 0.08$, $\mu_s = 0.12$).

* **El Reto:** Calcula la fuerza mínima para iniciar el movimiento, la fuerza para mantener velocidad constante, y la aceleración si un niño tira con $F = 80$ N a 20° sobre la horizontal.
* **Análisis Crítico:** ¿Por qué los pescadores humedecen el hielo antes de arrastrar los trineos? Relaciona con la capa de agua que reduce $\mu_k$ a ~0.02.
* **Simulación GeoGebra:** [Simulación de Rozamiento en Hielo](https://www.geogebra.org/m/W7KdWvYv) - Compara coeficientes de rozamiento y fuerzas requeridas.

---

### 🧠 Desafío 3
**La Cuerda del Alpinista en la Cordillera Blanca**

Un alpinista de $m = 65$ kg cae en una grieta y es detenido por la cuerda. La cuerda de nylon tiene $k = 1500$ N/m y se estira $\Delta x = 0.8$ m antes de detenerlo.

* **El Reto:** Calcula la velocidad del alpinista justo antes de que la cuerda se tense, la aceleración máxima durante el frenado, y la fuerza máxima que soporta la cuerda.
* **Análisis de Sensibilidad:** Las cuerdas de escalada modernas son dinámicas ($k$ variable). ¿Qué sucede si $k$ aumenta un 50%? ¿Es más seguro o más peligroso para el alpinista?
* **Simulación GeoGebra:** [Simulación de Caída con Cuerda Elástica](https://www.geogebra.org/m/XKfpRjQH) - Modela la absorción de energía en el frenado.

---

### 🧠 Desafío 4
**El Frenado de Emergencia del Bus Metropolitano**

Un bus de $m = 15000$ kg viaja a $v = 60$ km/h por la Vía Expresa. El conductor frena bloqueando ruedas ($\mu_k = 0.55$ sobre asfalto seco).

* **El Reto:** Calcula la distancia de frenado, el tiempo de detención, y la fuerza de rozamiento. Si el asfalto está mojado ($\mu_k = 0.30$), ¿cuál es la nueva distancia de frenado?
* **Toma de Decisión:** La normativa de transporte exige detenerse en menos de 40 m desde 60 km/h. ¿Cumple el bus en ambas condiciones? Propón medidas si no cumple.
* **Simulación GeoGebra:** [Simulación de Frenado con Rozamiento](https://www.geogebra.org/m/W7KdWvYv) - Varía la velocidad y el coeficiente de rozamiento.

---

### 🧠 Desafío 5
**La Grúa del Puerto del Callao**
Una grúa portuaria levanta un contenedor de $m = 3200$ kg con un cable de acero de $k = 5 \times 10^6$ N/m.

* **El Reto:** Calcula la tensión en el cable durante levantamiento a velocidad constante, la elongación del cable, y la aceleración máxima permitida si la tensión no debe exceder 1.5 veces el peso.
* **Extensión Creativa:** Diseña un sistema de amortiguación usando un resorte auxiliar que reduzca la elongación del cable principal en un 30%. ¿Qué constante elástica necesita el resorte auxiliar?
* **Simulación GeoGebra:** [Simulación de Sistema Grúa-Resorte](https://www.geogebra.org/m/XKfpRjQH) - Observa la elongación bajo diferentes condiciones de carga.

---

### 🧠 Desafío 6
**El Tobogán Acuático del Parque de las Aguas**

Un tobogán acuático tiene pendiente $\theta = 35°$, longitud $L = 25$ m, y coeficiente de rozamiento cinético con agua $\mu_k = 0.05$.

* **El Reto:** Calcula la velocidad en la base del tobogán partiendo del reposo, el tiempo de descenso, y la fuerza normal sobre una persona de $m = 60$ kg.
* **Evaluación:** Si el tobogán debe tener una velocidad máxima de seguridad de 12 m/s, ¿qué longitud máxima puede tener manteniendo el mismo ángulo?
* **Simulación GeoGebra:** [Simulación de Descenso con Rozamiento](https://www.geogebra.org/m/W7KdWvYv) - Ajusta el ángulo y la longitud del tobogán.

---

### 🧠 Desafío 7
**El Sistema de Poleas del Elevador de Carga**

Un sistema de poleas tiene configuración de polipasto con 4 tramos de cuerda sosteniendo una carga de $m = 500$ kg.

* **El Reto:** Calcula la tensión en cada tramo de cuerda si el sistema está en equilibrio, la fuerza necesaria para levantar la carga a velocidad constante, y la aceleración si se aplica una fuerza de $F = 1500$ N.
* **Interpretación Profesional:** ¿Por qué los polipastos industriales usan 6-8 tramos en lugar de 2-4? Relaciona con la seguridad y el desgaste de la cuerda.
* **Simulación GeoGebra:** [Simulación de Sistema de Poleas](https://www.geogebra.org/m/XKfpRjQH) - Visualiza la distribución de tensiones.

---

### 🧠 Desafío 8
**La Fuerza Centrífuga del Trompo Mecánico**

Un niño de $m = 30$ kg se sienta en un trompo mecánico que gira con $\omega = 2$ rad/s a $R = 2$ m del centro. El asiento está inclinado 15° hacia afuera.

* **El Reto:** En el sistema de referencia del trompo (no inercial), calcula la fuerza centrífuga ficticia, la fuerza de rozamiento estático necesaria para que el niño no se deslice, y el coeficiente mínimo $\mu_s$ requerido.
* **Análisis Crítico:** ¿Por qué los trompos reales tienen asientos inclinados hacia adentro en lugar de hacia afuera? Compara la estabilidad en ambas configuraciones.
* **Simulación GeoGebra:** [Simulación de Fuerzas en Sistema Rotatorio](https://www.geogebra.org/m/W7KdWvYv) - Observa la fuerza centrífuga y su efecto.

---

### 🧠 Desafío 9
**La Báscula del Mercado de Surquillo**

Un vendedor usa una báscula de resorte (dinamómetro) para pesar papas. El resorte tiene $k = 800$ N/m y se calibra para leer masa en kg.

* **El Reto:** Calcula la elongación para una bolsa de $m = 5$ kg, la frecuencia de oscilación natural del sistema, y el error de lectura si el vendedor pesa mientras el camión pasa vibrando el piso a $f_{vib} = 2$ Hz.
* **Análisis de Sensibilidad:** Si la constante del resorte se desgasta un 10% (disminuye), ¿qué error sistemático introduce en las lecturas de masa? ¿A favor del vendedor o del cliente?
* **Simulación GeoGebra:** [Simulación de Báscula de Resorte](https://www.geogebra.org/m/XKfpRjQH) - Modela la calibración y vibraciones.

---

### 🧠 Desafío 10
**El Equilibrio del Puente Colgante de los Suspiros**

Un modelo del Puente de los Suspiros tiene una cuerda central con un peso colgante de $m = 0.5$ kg. Las cuerdas laterales forman ángulos $\theta_1 = 50°$ y $\theta_2 = 40°$ con la horizontal (asimetría por viento).

* **El Reto:** Calcula la tensión en cada cuerda lateral usando el método del triángulo de fuerzas. Verifica el resultado por descomposición cartesiana.
* **Extensión Creativa:** Si el viento aumenta y cambia los ángulos a 60° y 30°, ¿cuál cuerda está más cerca de romperse? Diseña un sistema de alerta basado en la relación de tensiones.
* **Simulación GeoGebra:** [Simulación de Triángulo de Fuerzas](https://www.geogebra.org/m/W7KdWvYv) - Construye el triángulo de fuerzas interactivamente.

---s