# Modelación y Simulación 2025

Este es un curso introductorio a la modelación y simulación computacional, y en general al cómputo científico. Tiene como objetivo cubrir algunos temas relacionados con métodos numéricos computacionales, y se estudian algoritmos para cálculo científico y su implementación computacional. Se estudian tres grandes temas: 

(1) Optimización numérica continua y discreta.

(2) Modelación continua y discreta, principalmente mediante EDO.

(3) Simulación de fenómenos mediante distribuciones de probabilidad. 

La primera parte del curso se enfoca en introducir temas de optimización numérica. Iniciamos formulando problemas de programación lineal, y sus propiedades, e introducimos el algoritmo Simplex. Veremos aplicaciones de programación lineal en problemas de transporte y problemas de asignación. En seguida, hacemos una revisión de algunos métodos de optimización no lineal, principalmente los métodos de gradiente, así como métodos de la familia de gradiente conjugado y métodos quasi-Newton. El tema culmina una introducción a algunos métodos de optimización combinatoria y discreta, como por ejemplo los algoritmos genéticos, y algoritmos evolutivos y de partículas. 

En el segundo bloque, estudiamos modelos de ecuaciones diferenciales y sistemas de ecuaciones diferenciales: estudiamos algunas EDO y EDP clásicas, desde el enfoque de la construcción del modelo diferencial. Aprederemos algunas técnicas para analizar cualitativamente los modelos diferenciales, y aprenderemos algoritmos numéricos para la solución de EDOs y sistemas de EDOs. Introducimos algunos elementos de modelación con EPDs y un algoritmo de diferencias finitas para su solución numérica. En esta parte aplicamos las EDO y las EDP para modelar y simular fenómenos de dinámica de poblaciones, modelos ecológicos y modelos de difusión, aplicados a diferentes contextos. 

En la parte final del curso hacemos uso de distribuciones de probabilidad, para modelar aquellos fenómenos en los que interviene algún componente estocástico. Abordaremos algoritmos numéricos para la generación de muestras aleatorias de distribuciones de probabilidad, y aplicaremos estos algoritmos al estudio de ciertos problemas de modelación. Hacemos una revisión de teoría de colas, y cómo simularlas de forma computacional. Finalmente, introducimos algunos métodos de estadística bayesiana para simulación.

**Importante!!** El curso cuenta con una parte práctica extensiva, en la que el estudiante implementará en código computacional cada uno de los algoritmos estudiados. Parte fundamental del curso consiste en utilizar las herramientas aprendidas en varios proyectos aplicados donde se trabajará con datos reales y comunicar los resultados mediante reportes técnicos y seminarios.


# Prerrequisitos

Se recomienda que los estudiantes antes del curso estén habituados con los temas:
* Cálculo en una y varias variables
* Álgebra lineal y álgebra matricial
* Ecuaciones diferenciales ordinarias
* Probabilidad y estadística
* Un curso de Programación.


# Programa del curso
<div id='id-programa'/>

[Programa del curso](programa/Programa-sim2025.pdf){:target="_blank"}

### Horario
<div id='id-horario'/>

* Martes de 16:30 a 18:50 CIT-301, y Jueves de 17:20 a 18:50 CIT-215.

### Office Hours
<div id='id-office'/>

* Martes o jueves de 19:00 a 19:45.


# Material del curso
<div id='id-material'/>

**No.**  | **Fecha**    | **Tópicos**                                                   | **Recursos**
-------- | ------------ | ------------------------------------------------------------- |  ---------------------------------
01       | 03.07.2025   | Inicio del curso. Motivación de cómputo científico. <br/> [Aula 01](aulas/Aula01.pdf){:target="_blank"} |  
02       | 08.07.2025   | Programación Lineal. Región factible. Forma estándar.         | Taha, Cap. 1 <br/> Matousek-Gärner, Cap. 4
03       | 10.07.2025   | Variables básicas y no-básicas. Algoritmo Simplex.            | Taha, Cap. 2 y 3 <br/> Matousek-Gärner, Cap. 5 <br/> [Simplex.xlsx](code/Simplex.xlsx){:target="_blank"}
04       | 15.07.2025   | Formulación de problemas de PL. Uso de Julia o Python.        | [Ejemplo1.ipynb](code/Ejemplo1.ipynb){:target="_blank"} <br/> [Ejemplo3.ipynb](code/Ejemplo3.ipynb){:target="_blank"} <br/> [Ejemplo_Fábrica.ipynb](code/Ejemplo_Fábrica.ipynb){:target="_blank"} 
L1       | 17.07.2025   | Lab 01.                                                       | [Lab 01](labs/lab01.pdf){:target="_blank"} <br/> **Entrega: 24 de julio**  
05       | 22.07.2025   | Problemas de transporte. Problemas de asignación. <br/> | [Asignment.ipynb](code/Asignment.ipynb){:target="_blank"} <br/> [Transport.ipynb](code/Transport.ipynb){:target="_blank"}   
06       | 24.07.2025   | Métodos iterativos para calcular raíces: Bisección, Secante, método de Newton-Raphson.  | Burden-Faires, Secciones 2.1 a 2.4  
07       | 29.07.2025   | Método de Newton en varias variables. <br/>  | Burden-Faires, Sección 10.2
L2       | 29.07.2025   | Lab 02.                                                       | [Lab 02](labs/lab02.pdf){:target="_blank"} <br/> **Entrega: 5 de agosto**  
08       | 31.08.2025   | Optimización 1-dimensional. <br/>  [Aula 08](aulas/Aula08.pdf){:target="_blank"} | 
09       | 07.08.2025   | Optimización continua. Tipos de mínimos.  <br/>  [Aula 09](aulas/Aula09.pdf){:target="_blank"} | 
10       | 12.08.2025   | Descenso gradiente. Gradiente estocástico. <br/>  [Aula 10](aulas/Aula10.pdf){:target="_blank"} | [Stochastic Gradient Descent (SGD)](https://www.ruder.io/optimizing-gradient-descent/){:target="_blank"} 
11       | 12.08.2025   | Gradiente conjugado. Métodos Quasi-Newton: SR1, DPF, BFGS.  [Aula 11](aulas/Aula11.pdf){:target="_blank"} [Aula 12](aulas/Aula12.pdf){:target="_blank"} |  
L3       | 14.08.2025   | Lab 03.                                                       | [Lab 03](labs/lab03.pdf){:target="_blank"} <br/> [datos_lab3.csv](labs/datos_lab3.csv){:target="_blank"} <br/> **Entrega: 21 de agosto** 
12       | 19.08.2025   | Optimización discreta. Representación. <br/> [Aula 14](aulas/Aula14.pdf){:target="_blank"} |  
13       | 19.08.2025   | Algoritmos genéticos (GA). <br/> [Aula 15](aulas/Aula15.pdf){:target="_blank"} |  
14       | 21.08.2025   | Operadores de cruce y de mutación. Ejemplos GA. <br/> | Operadores para TSP <br/> [Larrañaga et al.](lectures/Larranaga_GA_for_TSP.pdf){:target="_blank"} 
L4       | 26.08.2025   | Lab 04.                                                       | [Lab 04](labs/lab04.pdf){:target="_blank"} <br/> **Entrega: 2 de septiembre.**
15       | 28.08.2025   | Búsqueda local, *Hill-Climbing*. <br/> [Aula 18](aulas/Aula18.pdf){:target="_blank"} |     
16       | 28.08.2025   | Enfriamiento simulado (*Simulated annealing*). <br/> [Aula 19](aulas/Aula19.pdf){:target="_blank"} |    
17       | 02.09.2025   | Ecuaciones diferenciales. Existencia y unicidad de soluciones. | [Apuntes EDO](lectures/Apuntes_EDO.pdf){:target="_blank"}   
18       | 04.09.2025   | Análisis cualitativo de EDO de 1er orden. <br/> | [Análisis Cualitativo](lectures/Analisis_Cualitativo.pdf){:target="_blank"}   
19       | 04.09.2025   | Campos de vectores. <br/> |    
20       | 09.09.2025   | Método de las isóclinas. Ecuaciones autónomas. <br/> |    
L5       | 11.09.2025   | Lab 05.                                                       | [Lab 05](labs/lab05.pdf){:target="_blank"} <br/> **Entrega: 25 de septiembre.**
21       | 23.09.2025   | Puntos de equilibrio en sistemas de EDO. <br/> |   
22       | 30.09.2025   | Solución numérica de EDOs. <br/> |   
23       | 02.10.2025   | Modelos de 1 población: Malthus, Logístico, Gompertz.  |   
24       | 07.10.2025   | Presentación del primer proyecto.  |   
25       | 09.10.2025   | Modelos de 2 poblaciones. Lotka-Volterra. Modelo SIR.  |   
L6       | 14.09.2025   | Lab 06.                                                       | [Lab 06](labs/lab06.pdf){:target="_blank"} <br/> **Entrega: 19 de octubre.**


# Proyectos
<div id='id-proyectos'/>

Durante el curso se realizarán dos proyectos. 

## Proyecto 1
<div id='id-proy1'/>

**No.**  | **Fecha**    | **Tópicos**                                   | **Recursos**
-------- | ------------ | --------------------------------------------- |  -------------------------------------
 1       | 26.08.2025   | Proyecto - *Algoritmos Genéticos + LP*        | [Proyecto 1](proyectos/Proyecto1.pdf){:target="_blank"} <br/> **Entrega: 07 de octubre.** 
 2       | 07.10.2025   | Presentación del proyecto.                    |  
 3       | 10.10.2025   | Entrega de código e informe final.            |  


## Proyecto 2
<div id='id-proy2'/>

**No.**  | **Fecha**     | **Tópicos**                                      | **Recursos**
-------- | ------------  | ------------------------------------------------ |  -------------------------------------
 1       | 16.10.2025    | Proyecto - *Modelación y Simulación*.            | [Proyecto](proyectos/Proyecto2.pdf){:target="_blank"} <br/> **Entrega: 22 de noviembre.** 
 2       | 04.11.2025    | Fecha límite para elección de tema.              |  
 3       | 17-21.11.2025 | Presentaciones.                                  |  
 4       | 22.11.2025    | Entrega de código, presentación e informe final. |  


## Horario Proyecto 1

**Hora**  | **Grupo**    
--------- | ------------ 
4:30      | Grupo 8
4:45      | Grupo 3
5:00      | Grupo 10
5:15      | Grupo 4
5:30      | Grupo 2
5:45      | Grupo 6
6:00      | Grupo 7
6:15      | Grupo 9
6:30      | Grupo 5
6:45      | Grupo 1
7:00      | Héctor Daniel Penedo

# Referencias
<div id='id-ref'/>

### Textos: 

* [S. Ross (2022). *Simulation*. 6th Ed.](https://libgen.li/ads.php?md5=173766bf2de3d62a9816564e7cda4239){:target="_blank"}

* [K. Atkinson, W. Han y D. Stewart (2009). *Numerical Solution of Ordinary Differential Equations*.](https://homepage.divms.uiowa.edu/~atkinson/papers/NAODE_Book.pdf){:target="_blank"}

* [H. Taha (2017). *Investigación de Operaciones*. 9a. Ed.](https://libgen.li/ads.php?md5=976e88a1d93760afbdf54160edc5ab5a){:target="_blank"}

### Referencias adicionales:

* [J. Matousek, B. Gärtner, (2007). *Understanding and Using Linear Programming*.](https://libgen.li/ads.php?md5=b760fdd2b747713ec1c8f24301fc2540){:target="_blank"}

* [R. Burden, A. Burden, D. J. Faires (2017). *Análisis numérico.*](https://libgen.li/ads.php?md5=8b84557e0b5a5c8effd22ce47bc2737f){:target="_blank"}

* [M. Martcheva (2010). *An Introduction to Mathematical Epidemiology*.](http://library.lol/main/B49DE076CF4518052FFBA1E0B8D3BD1F){:target="_blank"}

* [C. Robert y G. Casella (2004). *Monte Carlo Statistical Methods*.](http://library.lol/main/A910C1F6887E40EE92E4394860CFCAB8){:target="_blank"}

* [B. Zeigler, A. Muzy y E. Kofman (2019). *Theory of Modeling and Simulation*.](http://library.lol/main/E2ECE9CB0E7D0B070742712BF34FB081){:target="_blank"}

* [J. A. Sokolowski y C. M. Banks (2010). *Modeling and Simulation Fundamentals*.](http://library.lol/main/F4F7B06B2CFA15FD273DBFE01B09D8EA){:target="_blank"}
    

--- 
