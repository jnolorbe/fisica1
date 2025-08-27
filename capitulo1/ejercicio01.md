# Problema 1.2 
### **Modelado de la Velocidad de un Paracaidista**

Un paracaidista salta desde un avión. Para estudiar el movimiento de su caída, se ha medido su velocidad en función del tiempo. Los datos obtenidos, con las precisiones de medición indicadas, se muestran en la siguiente tabla.

**Se pide al estudiante:**

1.  **Graficar** los datos en un plano cartesiano, colocando la velocidad en el eje 'y' y el tiempo en el eje 'x'.
2.  **Describir** el movimiento del paracaidista a partir de la gráfica. 
3.  **Evaluar** los siguientes tres modelos matemáticos para describir la velocidad del paracaidista, seleccionando los mejores coeficientes.
    * **Modelo 1 (Lineal):** $$v(t) = at + b$$
    * **Modelo 2 (Exponencial Asintótico):** $$v(t) = A(1 - e^{-Bt})$$
    * **Modelo 3 (Polinómico de segundo grado):** $$v(t) = at^2 + bt + c$$
3.  **Comparar** el rendimiento de los tres modelos basándose en la predicción.
4.  **Seleccionar y justificar** cuál de los tres modelos es el más adecuado para representar el fenómeno físico.
5.  **Extrapolar** la velocidad del paracaidista a los 30 segundos utilizando el modelo seleccionado como el mejor. ¿Qué significa este valor físicamente?


Aquí están los datos para el problema:

| Tiempo (s) | Velocidad (m/s) |
| :--------- | :-------------- |
| 0.0        | 0.20             |
| 0.5        | 4.70             |
| 1.0        | 9.40             |
| 1.5        | 13.7            |
| 2.0        | 16.4            |
| 2.5        | 19.6            |
| 3.0        | 23.3            |
| 3.5        | 25.6            |
| 4.0        | 27.3            |
| 4.5        | 29.9            |
| 5.0        | 31.4            |
| 5.5        | 33.1            |
| 6.0        | 35.1            |
| 6.5        | 35.4            |
| 7.0        | 36.8            |
| 7.5        | 38.6            |
| 8.0        | 39.4            |
| 8.5        | 41.0            |
| 9.0        | 41.3            |
| 9.5        | 41.8            |
| 10.0       | 44.0            |
| 10.5       | 43.8            |
| 11.0       | 44.5            |
| 11.5       | 44.3            |
| 12.0       | 45.2            |
| 12.5       | 46.0            |
| 13.0       | 45.7            |
| 13.5       | 46.8            |
| 14.0       | 46.7            |
| 14.5       | 47.1            |
| 15.0       | 47.2            |
| 15.5       | 48.7            |
| 16.0       | 48.0            |
| 16.5       | 47.6            |
| 17.0       | 48.7            |
| 17.5       | 47.9            |
| 18.0       | 48.7            |
| 18.5       | 47.8            |
| 19.0       | 48.2            |
| 19.5       | 49.1            |
| 20.0       | 49.5            |

***

### **Solución y Guía Detallada**

#### **Paso 1: Análisis y Visualización de los Datos**

Al graficar los datos, se observa que la velocidad del paracaidista aumenta rápidamente al principio y luego la tasa de aumento disminuye progresivamente. A partir de los 15 segundos, la velocidad parece estabilizarse, acercándose a un valor constante. Este comportamiento se conoce como **velocidad terminal**.

#### **Paso 2: Formulación de Modelos Matemáticos**

Debido a que el gráfico muestra una curva que tiende a un valor límite en lugar de una línea recta, un modelo lineal ($$v = at+b$$) no sería apropiado. La física de la caída con resistencia del aire indica que el movimiento se describe mejor con un modelo exponencial de la forma:

$$v(t) = A(1 - e^{-Bt})$$

Donde:
* $$v(t)$$ es la velocidad en función del tiempo.
* $$A$$ representa la **velocidad terminal**, el valor máximo al que la velocidad tiende asintóticamente.
* $$B$$ es una constante relacionada con la resistencia del aire y la masa del paracaidista.

#### **Paso 3: Ajuste y Evaluación del Modelo**

Utilizando un método de ajuste no lineal (como el método de los mínimos cuadrados), se pueden encontrar los mejores valores para las constantes $$A$$y$$B$$. El ajuste de los datos arroja los siguientes parámetros para el modelo:

* **Parámetro A (Velocidad Terminal):** $$49.79 \text{ m/s}$$* **Parámetro B:**$$0.20 \text{ 1/s}$$

Esto nos da el modelo ajustado:

$$v(t) = 49.79(1 - e^{-0.20t})$$

Para evaluar la calidad del ajuste, se calcula el **coeficiente de determinación ($$R^2$$)**. Un valor de $$R^2$$ cercano a 1 indica que el modelo explica una gran parte de la variabilidad de los datos.

* **Coeficiente de Determinación ($$R^2$$):** $$0.9988$$

Este valor de $$R^2$$ tan cercano a 1 muestra que el modelo exponencial es una excelente representación matemática del fenómeno físico.

#### **Paso 4: Extrapolación**

Para predecir la velocidad a los 30 segundos, se utiliza el modelo ajustado con $$t = 30$$:

$$v(30) = 49.79(1 - e^{-0.20 \times 30})$$

$$v(30) = 49.79(1 - e^{-6})$$

$$v(30) = 49.79(1 - 0.00248)$$

$$v(30) = 49.67 \text{ m/s}$$

**Significado físico:** La extrapolación muestra que la velocidad a los 30 segundos es $$49.67 \text{ m/s}$$. Este valor es muy cercano a la velocidad terminal de $$49.79 \text{ m/s}$$. Esto significa que el paracaidista prácticamente ha alcanzado su velocidad máxima y su velocidad ya no cambiará significativamente de aquí en adelante, pues la fuerza de la resistencia del aire se ha equilibrado con la fuerza de la gravedad.