# taller-corte-2
# 📊 Análisis Estadístico Descriptivo — Apps Descargadas

> **Taller No. 3 | Inteligencia Artificial**  
> UNIVERSIDA DEL PACIFICO · Programa de Ingeniería de Sistemas · Semestre 8 – Corte II  
> Docente: WILMAN ANDRES QUIÑONES V.
> Estudiante: ISNILDO EQUIA PERTEAGA

---

## 📋 Tabla de Contenidos

1. [Introducción](#-introducción)
2. [Objetivo](#-objetivo)
3. [Metodología](#-metodología)
4. [Resultados — Tabla de Frecuencias](#-tabla-de-distribución-de-frecuencias)
5. [Representación Gráfica](#-representación-gráfica)
6. [Análisis e Interpretación](#-análisis-e-interpretación)
7. [Conclusiones](#-conclusiones)

---

##  Introducción

Este proyecto fue desarrollado como parte del Taller No. 3 de la asignatura de **Inteligencia Artificial**, con el fin de aplicar técnicas de **análisis estadístico descriptivo** sobre un conjunto de datos reales de uso de aplicaciones móviles.

El dataset contiene información de **50 usuarios** de distintos países de Latinoamérica (México, Colombia, Argentina, Chile y Perú), con diferentes niveles socioeconómicos. La variable de interés es **Apps Descargadas**, que registra el número de aplicaciones instaladas en el dispositivo de cada usuario.

Me pareció una variable muy relevante para analizar porque el número de aplicaciones que una persona tiene en su celular refleja directamente sus hábitos digitales, su nivel de consumo tecnológico y posiblemente su perfil socioeconómico. Organizar estos datos en una distribución de frecuencias me permitió descubrir patrones que no serían visibles al revisar los 50 valores uno por uno.

---

##  Objetivo

Aplicar técnicas de estadística descriptiva para **transformar los datos brutos de descargas de aplicaciones en información estructurada y visualmente interpretable**, que permita identificar patrones de comportamiento y apoyar la toma de decisiones en contextos tecnológicos y de negocio digital.

**Objetivos específicos:**
- Identificar la población, muestra, unidad de análisis y tipo de variable.
- Calcular los estadísticos básicos: mínimo, máximo y rango.
- Determinar el número de clases mediante la Regla de Sturges.
- Construir la tabla completa de distribución de frecuencias (fᵢ, hᵢ, Fᵢ, Hᵢ).
- Representar los datos mediante histograma, polígono de frecuencias y ojiva.
- Analizar e interpretar los resultados obtenidos.

---

##  Metodología

### Identificación del conjunto de datos

| Elemento | Descripción |
|---|---|
| **Población** | Todos los usuarios de aplicaciones móviles en Latinoamérica |
| **Muestra** | 50 usuarios registrados en el dataset |
| **Unidad de análisis** | Cada usuario individual (una fila del dataset) |
| **Variable** | Apps Descargadas — número de apps instaladas |
| **Tipo de variable** | Cuantitativa discreta |
| **Escala de medición** | Razón (tiene cero absoluto) |

### Cálculos previos

| Estadístico | Fórmula | Resultado |
|---|---|---|
| Total de observaciones | Conteo de registros | **n = 50** |
| Valor mínimo | min\{xᵢ\} | **Xmín = 30 apps** |
| Valor máximo | max\{xᵢ\} | **Xmáx = 132 apps** |
| Rango | R = Xmáx − Xmín | **R = 102 apps** |
| N.° de clases (Regla de Sturges) | k = 1 + 3.322 · log₁₀(n) = 1 + 3.322 · 1.699 = 6.64 | **k = 7 clases** |
| Amplitud de clase | A = ⌈R / k⌉ = ⌈102 / 7⌉ = ⌈14.57⌉ | **A = 15 apps** |

> 💡 **¿Por qué la Regla de Sturges?** Es uno de los criterios más utilizados en estadística descriptiva para determinar el número óptimo de clases. Evita tener demasiados intervalos vacíos (muy pocos datos) o intervalos tan amplios que oculten la distribución real de los datos.

---

## 📊 Tabla de Distribución de Frecuencias

**Tabla 1.** Distribución de frecuencias de la variable Apps Descargadas (n = 50).

| N° | Intervalo [Lᵢ – Lₛ) | Marca clase (mᵢ) | fᵢ | hᵢ | Fᵢ | Hᵢ |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | [30 – 45) | 37.5 | 7 | 0.1400 | 7 | 0.1400 |
| 2 | [45 – 60) | 52.5 | 6 | 0.1200 | 13 | 0.2600 |
| **3** | **[60 – 75)** | **67.5** | **10 ★** | **0.2000** | **23** | **0.4600** |
| 4 | [75 – 90) | 82.5 | 9 | 0.1800 | 32 | 0.6400 |
| 5 | [90 – 105) | 97.5 | 8 | 0.1600 | 40 | 0.8000 |
| 6 | [105 – 120) | 112.5 | 5 | 0.1000 | 45 | 0.9000 |
| 7 | [120 – 135) | 127.5 | 5 | 0.1000 | 50 | 1.0000 |
| **Total** | — | — | **50** | **1.0000** | **50** | **1.0000** |

> ** Clase modal:** el intervalo [60–75) es el de mayor frecuencia con fᵢ = 10 usuarios (20% del total).

### Interpretación de cada columna

- **Marca de clase (mᵢ):** valor central de cada intervalo, calculado como (Lᵢ + Lₛ) / 2. Representa estadísticamente a todos los datos del rango.
- **Frecuencia absoluta (fᵢ):** número de usuarios que caen en cada intervalo. La suma total debe ser n = 50 
- **Frecuencia relativa (hᵢ):** proporción de cada clase respecto al total (fᵢ / n). La suma debe ser 1.0000 
- **Frecuencia acumulada (Fᵢ):** suma progresiva de las fᵢ. El último valor siempre es n = 50 
- **Frecuencia relativa acumulada (Hᵢ):** proporción acumulada (Fᵢ / n). El último valor siempre es 1.0000 

---

##  Representación Gráfica

### Figura 1 — Histograma de Frecuencias Absolutas


**Análisis:** Al observar el histograma lo primero que noto es que las barras no tienen la misma altura, lo que confirma que la distribución no es uniforme. La barra más alta corresponde al intervalo **[60–75)** con 10 usuarios, lo que lo convierte en la clase modal. Hacia los extremos las barras disminuyen, especialmente los dos últimos intervalos que solo tienen 5 usuarios cada uno, generando una cola visible hacia la derecha. Esto es la primera señal de un **sesgo positivo** en la distribución.

---

### Figura 2 — Polígono de Frecuencias
<img width="1485" height="732" alt="image" src="https://github.com/user-attachments/assets/8c001640-5ab4-4c44-8ef7-1efe74dcb3e1" />

![Polígono de Frecuencias]
<img width="1485" height="732" alt="image" src="https://github.com/user-attachments/assets/3ef65974-6096-4f6e-b2bb-7540fa731430" />

**Análisis:** La curva del polígono sube hasta su punto máximo en la marca de clase **67.5** (intervalo [60–75)) y luego desciende de forma gradual. La bajada hacia la derecha es más lenta que hacia la izquierda, lo que confirma visualmente el sesgo positivo. La **media estimada x̄ ≈ 79.8 apps** supera a la marca de la clase modal (67.5), lo cual es la característica definitoria de una distribución con sesgo positivo: la presencia de usuarios con muchas apps eleva el promedio por encima del valor más frecuente.

---

### Figura 3 — Ojiva (Curva de Frecuencia Relativa Acumulada)

<img width="1468" height="731" alt="image" src="https://github.com/user-attachments/assets/10c709a0-55c2-400d-8118-eefdbee62c77" />

**Análisis:** La ojiva sube de forma más pronunciada en la parte central (donde se concentran la mayoría de los datos) y se aplana en los extremos. Las líneas de referencia muestran que:
- El **50% de los usuarios** tiene menos de ~78 apps (mediana estimada).
- El **80% de los usuarios** tiene menos de 105 apps — umbral estratégico clave.
- Solo el **10% de los usuarios** supera las 120 apps (segmento intensivo).

---

##  Análisis e Interpretación

###  Pregunta 1 — ¿Cuál es el intervalo con mayor concentración de observaciones?

El intervalo **[60–75) apps** es el de mayor concentración con **fᵢ = 10 usuarios**, lo que representa el **20% de la muestra**. Este intervalo es la **clase modal** de la distribución. Desde mi punto de vista, este rango tiene mucho sentido: corresponde a un usuario típico de smartphone que tiene instaladas las apps de redes sociales, mensajería, streaming, banca, mapas y algunas de entretenimiento, sin llegar a ser un usuario extremo. Si uno este intervalo con el siguiente [75–90) con 9 usuarios, más del **38% de la muestra** se concentra entre 60 y 90 apps.

---

###  Pregunta 2 — ¿La distribución parece uniforme, normal o sesgada?

La distribución **no es uniforme ni perfectamente normal**. Presenta un **sesgo positivo (hacia la derecha)**, aunque moderado. La evidencia es clara:

- La media estimada (~79.8 apps) es **mayor** que la marca de la clase modal (67.5 apps).
- En una distribución simétrica, media y moda deberían coincidir.
- Los dos últimos intervalos [105–120) y [120–135) mantienen 5 usuarios cada uno, generando una cola derecha visible.

En mi opinión, este sesgo se explica porque existe un grupo pequeño de usuarios muy activos digitalmente que tienen más de 105 apps instaladas, lo que "jala" el promedio hacia arriba respecto al valor más común.

---

###  Pregunta 3 — ¿Qué porcentaje de usuarios se encuentra por debajo de un nivel de descargas?

Usando la columna Hᵢ y la ojiva:

| Umbral | % de usuarios acumulado | Usuarios (de 50) |
|:---:|:---:|:---:|
| Menos de 45 apps | 14% | 7 |
| Menos de 60 apps | 26% | 13 |
| Menos de 75 apps | 46% | 23 |
| Menos de 90 apps | 64% | 32 |
| **Menos de 105 apps** | **80% (P₈₀)** | **40** |
| Menos de 120 apps | 90% | 45 |

El dato más relevante: el **P₈₀ ≈ 105 apps**, es decir, el 80% de los usuarios no supera las 105 aplicaciones. Si una empresa quiere llegar al grueso de sus usuarios, debe enfocarse en personas que manejan hasta 105 apps.

---

###  Pregunta 4 — ¿Qué información aporta la ojiva para la toma de decisiones?

La ojiva fue la herramienta que más me gustó construir porque es la más útil para tomar decisiones reales:

1. **Identificación de percentiles:** Puedo estimar visualmente la mediana (P₅₀ ≈ 78 apps) y cualquier otro percentil sin cálculos adicionales.
2. **Segmentación estratégica:** La ojiva revela tres grandes segmentos de usuarios:
   -  **Básicos** (0–60 apps): 26% de usuarios
   -  **Estándar** (60–105 apps): 54% de usuarios ← segmento principal
   -  **Intensivos** (>105 apps): 20% de usuarios
3. **Definición de umbrales:** Si quiero cubrir al 80% del mercado, el tope es 105 apps. Para el 90%, necesito llegar a 120 apps.
4. **Comparaciones futuras:** Si con otra muestra o en otro semestre repito el análisis, puedo superponer las ojivas y ver si el comportamiento cambió.

---

###  Pregunta 5 — ¿Qué conclusiones sobre el comportamiento de las descargas de aplicaciones?

- **Comportamiento heterogéneo pero concentrado:** El rango es amplio (30–132 apps), pero la mayoría (54%) se agrupa entre 60 y 105 aplicaciones.
- **El 20% intensivo es estratégicamente valioso:** Los usuarios con más de 105 apps consumen más servicios digitales y generan más datos de comportamiento.
- **La media no es el mejor indicador:** Dado el sesgo positivo, la **mediana (~78 apps) representa mejor al usuario típico** que el promedio (79.8 apps). Las decisiones basadas solo en el promedio podrían no ajustarse bien a la mayoría.
- **Tres segmentos de mercado claramente diferenciados:** Básico, estándar e intensivo, cada uno con estrategias de retención y monetización distintas.

---

##  Conclusiones

**1. La tabla de frecuencias como herramienta organizadora**  
Sin esta organización sería muy difícil identificar patrones en 50 datos. La Regla de Sturges me dio un criterio objetivo para decidir cuántos intervalos usar (k = 7), y la amplitud de 15 apps permitió que los datos quedaran bien distribuidos sin que ningún intervalo quedara vacío.

**2. El intervalo modal como punto de referencia**  
El intervalo [60–75) apps concentra al 20% de los usuarios. Es el dato más concreto del análisis: si alguien me pregunta cuál es el "usuario típico" de este dataset, puedo decir que tiene entre 60 y 74 aplicaciones instaladas.

**3. El sesgo positivo como señal de diversidad digital**  
La distribución sesgada hacia la derecha refleja la diversidad real en los hábitos digitales. Pocos usuarios con muchas apps son suficientes para desplazar la media. Esto es importante: **una empresa que base sus decisiones solo en el promedio podría diseñar productos que no se ajusten bien a la mayoría de sus usuarios.**

**4. La ojiva como herramienta de decisión**  
De todas las representaciones, la ojiva fue la más útil en términos prácticos. Saber que el 80% de los usuarios tiene menos de 105 apps orienta directamente decisiones de segmentación y focalización de recursos sin necesidad de cálculos adicionales.

**5. Reflexión final**  
Este taller me enseñó que detrás de cualquier conjunto de datos existe una historia que contar. La estadística descriptiva es la herramienta que nos permite descubrir esa historia de forma objetiva. En el campo de la inteligencia artificial, donde trabajamos constantemente con datos, dominar estas técnicas es un paso indispensable antes de aplicar cualquier modelo más complejo.

---

##  Referencias

- Devore, J. L. (2016). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Cengage Learning.
- Walpole, R. E., Myers, R. H., & Myers, S. L. (2012). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Pearson.
- Sturges, H. A. (1926). The choice of a class interval. *Journal of the American Statistical Association*, 21(153), 65–66.
- Quiñonez V., W. A. (2026). *Taller No. 3 – Análisis Estadístico Descriptivo y Visualización de Datos*. Universidad del Pacífico.

---

<div align="center">

**Universidad del Pacífico · Ingeniería de Sistemas · Inteligencia Artificial**  
Semestre 8 – Corte II · Junio 2026

</div>
