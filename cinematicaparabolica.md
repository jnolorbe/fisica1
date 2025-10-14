# Movimiento parabólico
---
## 📌 Problemas Resueltos
### Problema 1
```{admonition}  lanzamiento horizontal
:class: important
Determinar la velocidad horizontal mínima con la que debe ser lanzado un cuerpo para que pueda superar el obstáculo B.

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/cinematica01.png
:alt: lanzamiento horizontal
:width: 100%
:align: center
```

```{admonition} Solución
:class: dropdown hint

1. **Deducimos el tiempo de caída de A a B**. El tiempo de caída de un cuerpo en caída libre puede ser obtenido analizando el componente _y_ del movimiento, reempazando los datos en la cecuación de la posicón vertical:

    $y = y_0 + \vec{v}_{oy} t + \frac{1}{2} \vec{a_y}t^2$

    Reemplazando, $y = 15 \, m$, $y_o = 27\, m$, $\vec{v}_{oy} = 0$ y $\vec{a_y} = -g = -9.8 \, m/s^2$, el tiempo de caída es:

    $15 = 27 - 4.9 t^2 $

    $t = 1.56 \, s$

2. **Calulamos la velocidad mínima horizontal**. En el mismo intervalo de tiempo que el cuerpo cae de A a B, este debe recorrer una distancia horizontal mínima de $31 \, m$, por lo tanto su velocidad horizontal mínima es: 

    $ v_x =  \frac{x}{t} =  \frac{31}{1.56}$

    $ v_x \approx 20 \, m/s$

---
_✨ **Sintésis:** Siempre que el cuerpo supere una velocidad horizontal $v_x \approx 20 \, m/s$, el cuerpo logrará superar la distancia horizontal de $31 \, m$ entre A y B._ 
 
```
---
### Problema 2

```{admonition} Curva de seguridad 
:class: important

Un cañon dispara proyectiles con una rapidez de $100 m/s$, un dron es observado en la posición $(500m; 200m)$ con respecto al cañon. Deducir si es posible derribar al dron de un disparo. 

```

```{admonition} Solución
:class: dropdown hint
1. **Expresamos la ecuación de la trayectoria del proyectil**. Para diferentes ángulos de lanzamiento con una misma rapidez de disparo, se trazarán diferentes trayectorias, parabólicas, como se muetsra en la figura. Deduciremos si existe algún ángulo de disparo cuya trayectoria parabólica para por la posición del dron $(500m; 200m)$.  
    
    Ecuaciones cinemáticas del movimiento del proyectil:

    $x = v_o cos \theta \, t$

    $y = v_o sen \theta \, t - \frac{1}{2} g \,t^2$

    Combinando estas ecuaciones, obtenemos la ecuación de la trayactroria parabólica para distintos ángulos de lanzamiento: 
    
    \begin{equation*}
    y =x  \, tan \theta  -  \frac{1}{2} \frac{g}{v_o^2 cos^2  \theta} x^2
    \end{equation*}

    En la gráfica se muestra las trayectorias parabólicas del proyectil para diferentes ángulos de disparo. Dependiendo de la posición del dron, este podría estar fuera del alcance del proyectil,  $P_1$, o dos posibles ángulos, $P_2$ o un solo posible ángulo,  $P_3$.

    ```{figure} http://www.sc.ehu.es/sbweb/fisica_/cinematica/curvilineo/parabolico/parabolico2.gif
    :alt: Posibles Trayectorias parabolicas
    :width: 100%
    :align: center

2. **Deducimos el ángulo de disparo.** Para dedicro el ángulo de disparo, reemplazamos la coordenada del dron $(x = 500m; y = 200m)$ en la ecuación de la trayectoria parabólica del paso anterior:

    $200 = 500 \, tan \theta -  \frac{1}{2} \frac{9.8}{100^2 cos^2  \theta} 500^2$
    
    $200 = 500 tan \theta -  122.5 sec^2  \theta$
    
    $200 = 500 tan \theta -  122.5 (tan^2  \theta + 1)$

    $tan^2  \theta - 4.082 \, tan\theta + 2.633 = 0 $
    
    Esta es una ecuación cuadrática, $z = tan\theta $ cuya soluciones son:

    $z^2 - 4.082 \,z + 2.633 = 0 $

    $z = tan\theta = -  \frac{4.082 - \sqrt{4.082^2 - 4(2.633)}}{2}$

    $tan\theta_1 = 3.278  \, \longrightarrow   \, \theta_1 \approx 73\degree$

    $tan\theta_2 = 0.803 \, \longrightarrow   \, \theta_2 \approx 39\degree$

---
_✨**Sintésis:** Para un proyectil con una velocidad disparo determinada, la posibilidad de dar con un objetivo depende del ángulo de disparo. Todas las trayectorias parabólicas del proyectil estan inscritas en una **_curva de seguridad_**. Si el objetivo esta muy lejos o fuera de curva de seguridad el proyectil no podra dar con éste y si el objetivo esta dentro de la curva de seguridad, es posible que exista uno o dos ángulos para dar en el blanco. Para el caso resuelto hay dos ángulos para dar con el dron, $73\degree$ y $39\degree$. ¿Que forma tiene la curva de seguridad? ¿Cuáles serían los ángulos de disparo, si el dron se hubiera posicionado en $(x = 500m; y = 500m)$_

---
```

---
### Problema 3

```{admonition} Alcance máximo 
:class: important

Se disparan proyectiles desde un acantilado de altura  $ h = 250 \, m$ hasta barcos enemigos ubicados en el mar. El proyectil puede ser disparado con una velocidad de $v_o = 100 \, m/s$, deducir hasta que distancia del acantilado pueden acercarse los barcos y estar seguros de no ser alcanzado por lo proyectiles. 

```{figure} http://www.sc.ehu.es/sbweb/fisica3/cinematica/tarzan/alcance1.gif
:alt: Alcance horizontal
:width: 80%
:align: center
```

```{admonition} Solución
:class: dropdown hint
1. **Expresamos las ecuación paramétricas de la trayectoria del proyectil**. La posición $(x,y)$ del proyectil en función del tiempo esta dado por: 

    $x = v_o cos \theta \, t$

    $y = h + v_o sen \theta \, t - \frac{1}{2} g \,t^2$

2. **Calculamos el tiempo de vuelo $T$**. El tiempo de vuelo $T$ se obtiene cuando $y=0$ en la segunda ecuación y despejando el tiempo $T$.
    \begin{equation*}
    T = \frac{v_o}{g} \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right);  \, z = \frac{gh}{v_o^2}
    \end{equation*}

3. **Calculamos el alcance horizontal $R$**. Reemplanzando el tiempo de vuelo $T$ en la primera ecuación para calcular el alcance horiozontal $R$.
    \begin{equation*}
    R = \frac{v_o}{g} \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right) cos \theta
    \end{equation*}

4. **Deducimos el alcance horizontal máximo $R_{max}$**. Parta encotrar el ángulo que hace que el alcance horizontal sea máximo, derivamos $R$ con respecto a $\theta$ e igualamos la derivada a cero.
   
    \begin{equation*}
    \frac{d R}{d \theta} = \frac{d}{d \theta}  \left[ \frac{v_o}{g} \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right) cos \theta \right] = 0 \\
    \end{equation*}
    \begin{equation*}
    \frac{v_o}{g} \left( cos \theta + \frac{2 sen \theta cos \theta} {2 \sqrt{sen^2 \theta + 2z}} \right) cos \theta - \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right) sen \theta = 0
    \end{equation*}
   
    Expresamos en función de la $ tan \theta$ y despejamos:
   
    \begin{equation*}
    tan \theta = \frac{1}{\sqrt{1 + 2z}} = \frac{v_o}{\sqrt{v_o^2 + 2gh}}
    \end{equation*}
   
    Para los valores $v_o = 100 \, ms^{-1}$, $h = 250 \, m$ y $g = 9.8 \, ms^{-2}$ el ángulo de alcance máximo es:  

    $tan \theta = 0.819  \rightarrow \theta = 39\degree $
   
    Reemplazando este ángulo en la ecuación de alcance horizontal del paso (3):  
   
    $ R_{max} = 124. 6  \, m $

---
_✨**Sintésis:** Para un proyectil lanzado desde una cierta altura, existe un ángulo de alcance horizontal máximo. Una estrategia para deducir este ángulo es derivar la ecuación del alcance horizontal en función del ángulo de disparo e igualar a cero. Una vez obtenido este ángulo se deduce el alcance horizontal máximo. En este caso para los valores dados el ángulo de alcance horizontal máximos es aproximadamente $39\degree$ lo que da un alcance $R_{max} = 124.6 \, m$._

---
```

---


## 💡 Ejercicios propuestos

1. Un avion que vuela a una altura  $ h = 3500 \, m$ con una velocidad crucero de $v_o = 800 \, km/h$, deja caer una bomba. Deduducir la distancia horizontal que alcanza la bomba.
