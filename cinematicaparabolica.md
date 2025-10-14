# Movimiento parabólico
---
## 📌 Problemas Resueltos
### Problema 1
```{admonition}  lanzamiento horizontal
:class: important
Determinar la velocidad horizontal mínima con la que debe ser lanzado un cuerpo para que pueda superar el obstáculo B.

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/parabolico01.png
<<<<<<< HEAD
:alt: cinematica
:width: 60%
=======
:alt: lanzamiento horizontal
:width: 100%
>>>>>>> bfc03c1dd6c35a8efbd5aa14c08aaf391db060f3
:align: center
```

```{admonition} Solución
:class: dropdown hint

1. **Calculamos el tiempo de caída de A a B**. El tiempo de caída de un cuerpo en caída libre puede ser obtenido analizando solo el componente vertical del movimiento. 

    $y = y_o + v_{oy} t - \frac{1}{2} g t^2$

    Reemplazando, $y = 15 \, m$, $y_o = 27\, m$, $v_{oy} = 0$ y $ g = 9.8 \, m/s^2$, el tiempo que demora en caer es:

    $15 = 27 - 4.9 t^2 $

    $t = 1.56 \, s$

2. **Calulamos la velocidad mínima horizontal**. En el mismo intervalo de tiempo que el cuerpo cae de A a B recorre una distancia horizontal mínima de $d = 31 \, m$, por lo tanto su velocidad horizontal mínima es: 

    $ v_x =  \frac{d}{t} =  \frac{31}{1.56}$

    $ v_x \approx 20 \, m/s$

---
_✨ **Sintésis:** Al lanzar el cuerpo horizontalmente, el tiempo que demora en caer desde $y_A = 27\, m$ hasta $y_B = 15 \, m$ es $t = 1.56 \, s$, en ese mismo intervalo de tiempo debe recorrer al menos una distancia horizontal  $d = 31 \, m$ para sobre pasar el obstáculo, por lo tanto su velocidad horizontal mínima se obtiene divididendo la distancia horizontal entre el tiempo que demora en recorrerla, $v_x \approx 20 \, m/s$_ 
 
```
---
### Problema 2

```{admonition} Curva de seguridad 
:class: important

Un cañon ubicado en una superficie plana horizontal, puede disparar proyectiles con una rapidez de $100 m/s$ en diferentes direcciones. Un drone se acerca hasta la posición $(500m; 200m)$ con respecto al cañon. Deducir si es posible derribar al dron de un disparo. 

```

```{admonition} Solución
:class: dropdown hint

1. **Bosquejamos las trayectorias posibles del proyectil**. En la figura se muestra las trayectorias parabólicas del proyectil para diferentes ángulos de disparo. Dependiendo de la posición del drone, este podría estar fuera del alcance del proyectil o podría ser alcanzado por éste. Si el drone se encontrará en $P_1$ no hay forma que el proyectil lo alcance, si se encontrará en $P_2$ es posible que existan dos ángulos de disparos que den con el drone, y si se encontrará en $P_3$ es posible que solo exista un ángulo.

    ```{figure} http://www.sc.ehu.es/sbweb/fisica_/cinematica/curvilineo/parabolico/parabolico2.gif
    :alt: Posibles Trayectorias parabolicas
    :width: 100%
    :align: center

2. **Expresamos las ecuaciones paramétricas de la trayectoria del proyectil**. La posición $(x,y)$ del proyectil en función del tiempo esta dado por:
    
    $x = v_o cos \theta \, t$

    $y = v_o sen \theta \, t - \frac{1}{2} g \,t^2$

    Combinando estas ecuaciones, obtenemos la ecuación de la trayectoria parabólica para distintos ángulos de lanzamiento: 
    
    \begin{equation*}
    y =x  \, tan \theta  -  \frac{1}{2} \frac{g}{v_o^2 cos^2  \theta} x^2
    \end{equation*} 

3. **Deducimos el ángulo de disparo**. En la ecuación de la trayectoria que hemos obtenido sustituimos la coordenada del drone $(x = 500m; y = 200m)$:

    $200 = 500 \, tan \theta -  \frac{1}{2} \frac{9.8}{100^2 cos^2  \theta} 500^2$
    
    $200 = 500 \, tan \theta -  122.5 sec^2  \theta$
    
    $200 = 500 \, tan \theta -  122.5 (tan^2  \theta + 1)$

    $tan^2  \theta - 4.082 \, tan\theta + 2.633 = 0 $
    
    Esta es una ecuación cuadrática, $z = tan\theta $ cuya soluciones son:

    $z^2 - 4.082 \,z + 2.633 = 0 $

    $z = tan\theta = -  \frac{4.082 - \sqrt{4.082^2 - 4(2.633)}}{2}$

    $tan\theta_1 = 3.278  \, \longrightarrow   \, \theta_1 \approx 73\degree$

    $tan\theta_2 = 0.803 \, \longrightarrow   \, \theta_2 \approx 39\degree$

---
_✨**Sintésis:** Para un proyectil con una velocidad disparo determinada todas las trayectorias parabólicas del proyectil estan inscritas en una **_curva de seguridad_**. Si el objetivo esta fuera de curva de seguridad el proyectil no podra dar con éste y si el objetivo esta dentro de la curva de seguridad, es posible que exista uno o dos ángulos para dar en el blanco. Para el problema resuelto hay dos ángulos de disparo que pueden dar con el drone, $73\degree$ y $39\degree$. ¿Que forma tiene la curva de seguridad? ¿Cuáles serían los ángulos de disparo, si el drone se encontrará en $(x = 500m; y = 500m)$_

---
```

---
### Problema 3

```{admonition} Alcance máximo 
:class: important

Se disparan proyectiles desde un acantilado de altura  $ h = 250 \, m$ hasta barcos enemigos ubicados en el mar. El proyectil puede ser disparado con una velocidad de $v_o = 100 \, m/s$, deducir hasta que distancia horizontal $R$ del acantilado pueden acercarse los barcos y estar seguros de no ser alcanzado por los proyectiles. 

```{figure} http://www.sc.ehu.es/sbweb/fisica3/cinematica/tarzan/alcance1.gif
:alt: Alcance horizontal
:width: 80%
:align: center
```

```{admonition} Solución
:class: dropdown hint
1. **Expresamos las ecuaciones paramétricas de la trayectoria del proyectil**. La posición $(x,y)$ del proyectil en función del tiempo esta dado por: 

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

4. **Deducimos el alcance horizontal máximo $R_{max}$**. Parta encontrar el ángulo que hace que el alcance horizontal sea máximo, derivamos $R$ con respecto a $\theta$ e igualamos la derivada a cero.
   
    \begin{equation*}
    \frac{d R}{d \theta} = \frac{d}{d \theta}  \left[ \frac{v_o}{g} \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right) cos \theta \right] = 0 \\
    \end{equation*}
    \begin{equation*}
    \frac{v_o}{g} \left( cos \theta + \frac{2 sen \theta cos \theta} {2 \sqrt{sen^2 \theta + 2z}} \right) cos \theta - \left(sen \theta + \sqrt{sen^2 \theta + 2z} \right) sen \theta = 0
    \end{equation*}
   
    Resolvemos y  despejamos $ tan \theta$:
   
    \begin{equation*}
    tan \theta = \frac{1}{\sqrt{1 + 2z}} = \frac{v_o}{\sqrt{v_o^2 + 2gh}}
    \end{equation*}
   
    Para los valores $v_o = 100 \, ms^{-1}$, $h = 250 \, m$ y $g = 9.8 \, ms^{-2}$ se tiene:  

    $tan \theta = 0.819  \rightarrow \theta = 39\degree $
   
    Reemplazando este ángulo en la ecuación de alcance horizontal del paso (3):  
   
    $ R_{max} = 124. 6  \, m $

---
_✨**Sintésis:** Para un proyectil lanzado desde una cierta altura, existe un ángulo de alcance horizontal máximo. Una estrategia para deducir este ángulo es derivar la ecuación del alcance horizontal en función del ángulo de disparo e igualar a cero. Una vez obtenido este ángulo se deduce el alcance horizontal máximo. En este caso el ángulo de alcance horizontal máximo es aproximadamente $39\degree$ lo que da un alcance horizontal máximo $R_{max} = 124.6 \, m$._

---
```

---


## 💡 Ejercicios propuestos

<<<<<<< HEAD
1. Un avión de provisiones vuela a una altura  $ h = 3500 \, m$ con una velocidad horizontal crucero de $v_o = 800 \, km/h$ ¿en que momento debe dejar caer las provisiones para que estas lleguen a su objetivo?

2. Un jugador patea una pelota con una velcoidad de $10 \,m/s$. Deducir la distancia horizontal máxima que puede lograr.

3. Un proyectil es lanzado en un plano inclinado, como muestra la figura. Si la velocidad de disparo es $ v_0 = 60 \,  m/s$, la pendiente del plano inclinado $\alpha = 20 \degree$ y el ángulo de disparo con respecto a la horizontal es $\theta = 10 \degree$, deducir el alcance $R$ del proyectil. 

```{figure} http://www.sc.ehu.es/sbweb/fisica/cinematica/parabolico/alcance1/alcance2.gif
:alt: Lanzamiento en plano inclinado
:width: 60%
:align: center
**Referencia** http://www.sc.ehu.es/
```
4. Se lanza horizontalmente un proyectil desde una altura  $ h = 25 \, m$ con una velocidad horizontal $v_o = 10 \, m/s$. Si consideramos la fricción del aire, el proyectil esta acelerado en la horizontal con $a_x = -4 \, m/s^2$ y en la vertical con $a_y = -6 \, m/s^2$, deducir la distancia horizontal que alcanza el proyectil al llegar al suelo. 

5. Dos cañones se apuntan directamente, como se muestra en la figura. Al dispararse, las balas de cañón seguirán las trayectorias mostradas; P es el punto donde se cruzan. Si queremos que las balas de los cañones impacten entre sí, ¿deberían los artilleros disparar primero el cañón A, primero el cañón B o simultáneamente? Ignore los efectos debidos a la resistencia del aire.

```{figure} https://github.com/jnolorbe/fisica1/blob/main/figuras/enfrentamiento.png
:alt: enfrentamiento
:width: 100%
:align: center
```
=======
1. Un avion que vuela a una altura  $ h = 3500 \, m$ con una velocidad crucero de $v_o = 800 \, km/h$, deja caer una bomba. Deduducir la distancia horizontal que alcanza la bomba.
>>>>>>> bfc03c1dd6c35a8efbd5aa14c08aaf391db060f3
