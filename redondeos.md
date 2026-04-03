# Redondeos
---
## ✏️ Reglas sencillas para operaciones

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

## 📌 Problemas Resueltos

### Problema 1

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
<!-- /figuras/vasosgraduados.png -->

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
* 🟢 **Verde (Validación):** El resultado $1130 \, \text{ml}$ refleja la realidad de la medición; la "vaguedad" del segundo frasco domina el resultado.
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

### Problema 2

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
1. **Cálculo bruto:** $R = 1.35 \, \text{V} / 2.9 \, \text{A} = 0.46551724 \, \Omega$

2. **Análisis de Cifras Significativas (C.S.):**
   - $V = 1.35$ (3 C.S.)
   - $I = 2.9$ (2 C.S.)

   > _**Regla Crítica:** Al multiplicar o dividir, el resultado se redondea al mismo número de cifras significativas que la cantidad que tenga menos._

3. **Resultado:** Como la corriente tiene solo 2 C.S., el resultado debe tener 2 C.S.
   **$R = 0.47 \, \Omega$**

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

### Problema 3

```{admonition}  Área circular
:class: important
Se mide el diámetro de una pila con un vernier, obteniendo $d = 19.95 \, \text{mm}$. Queremos hallar el área superficial ($A = \pi d^2 / 4$). 
**Pregunta de reflexión:** Si $\pi$ tiene infinitos decimales en la memoria de la calculadora, ¿cuántos de ellos "hereda" mi resultado final?

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/vernierdiametro.jpg
:alt: diametro con vernier
:width: 50%
:align: center
```
<!--/figuras/vernierdiametro.jpg  -->

```{admonition} Solución
:class: dropdown hint

En este nivel, el reto para un ingeniero no es solo contar cifras de las medidas, sino entender cómo las constantes matemáticas ($\pi$) y los números exactos (como el $1/2$ en las fórmulas de cinemática) afectan —o no— la precisión del resultado.

1. **Identificación de Datos:**

Diámetro ($d$): $19.95 \, \text{mm}$ (4 Cifras Significativas).

Constantes ($\pi$, $4$): Son números exactos o con precisión muy superior a la medida. No limitan la precisión.

2. **Cálculo Bruto:**
$A = \frac{\pi \cdot (19.95)^2}{4} = 312.5904325... \, \text{mm}^2$

3. **Criterio de Ingeniería:**
Como la medida más restrictiva es el diámetro (4 C.S.), el área debe reportarse con 4 C.S.

4. **Resultado Final:**
$A = 312.6 \, \text{mm}^2$

✍️  **Hazlo Tú: Calculos con Fórmulas Físicas**
Identifica que resultados son coreccto o incorrectos, justifica tu respuesta.
- Volumen  = V = $(1.23 \, cm)(1.7 \, cm)(2.345 \, cm)$ = 4.9 \, \text{cm}^3$
- Velocidad = V = $(1.25 \, m/s^2)(24.56 \, s)$ = $31 \, \text{m/s}$ 
- Altura = H = $(0.5)(9.81 \, m/s^2)(1.255 \, s)^2$ =  $7.73 \, \text{m}$
- Altura = H = $(0.5)(9.8 \, m/s^2)(1.255 \, s)^2$ = $7.7 \, \text{m}$

💡 **Conclusión**
Nota la diferencia entre los ejercicios 3 y 4. Un cambio en la precisión de la constante de gravedad ($9.81$ vs $9.8$) cambió totalmente la validez de tu resultado. Como ingeniero, siempre debes elegir constantes que tengan, al menos, la misma cantidad de cifras significativas que tus mediciones de campo.

```
---

## 🌀 **Recordar**

- **¡Nunca uses todas las cifras de la calculadora!** La calculadora no sabe la precisión de tus mediciones. Expresar un resultado con más cifras
de las que son significativas es una forma de reportar una precisión que no tienes.

- **Distingue las reglas:** **¡No es lo mismo!**. La regla para suma y resta se centra en las _posiciones decimales_ (los dígitos a la derecha del punto), mientras que la regla para multiplicación y división se centra en el número total de _cifras significativas_ (todos los dígitos importantes).

- **Entiende el 'porqué':** La razón es que la precisión del resultado de una operación entre cantidades físicas no puede exceder la precisión de la medida menos precisa.  Es decir, la precisión del resultado está siempre limitada por el dato menos preciso.

- **Redondea solo al final:** Realiza todos los cálculos con las cifras que te da la calculadora (o incluso con alguna extra), y redondea el resultado final solo al final, según 
la regla apropiada. Esto te ayuda a evitar errores de redondeo en los pasos intermedios.

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


---
## 🎯 [¡Autoevaluate!](https://gemini.google.com/share/3c61a48a100e)
