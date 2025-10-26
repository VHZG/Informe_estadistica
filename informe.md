![Portada](image.png)
ESTADÍSTICA
Título: Análisis de la evolución de la esperanza de vida
de hombres y mujeres en la Comunidad de Madrid
( 1986 – 2023 )
Autor: Gerardo Antonio Valdez Hernández
Profesor: José Ramón Hilera González

Contenido
Comunidad de Madrid (1986 – 2023) Título: Análisis de la evolución de la esperanza de vida de hombres y mujeres en la
Introducción
Contexto
Objetivo
Alcance.......................................................................................................................
Metodología
Origen de los datos
Herramientas..............................................................................................................
Diseño
Resultados
Medidas estadísticas
Tablas de contingencia
Diagramas
Análisis de resultados
Conclusiones
Referencias

Introducción
Contexto
Se presentan los datos correspondientes a la evolución de la esperanza de vida de
mujeres y hombres en la Comunidad de Madrid desde el año 1986 hasta el 2023.
Estos datos están registrados en dos grupos diferentes diferenciados según el sexo,
y muestran la edad media de esperanza de vida en cada una de las filas.

Objetivo
El objetivo de esta investigación es realizar un análisis estadístico descriptivo de la
edad media de esperanza de vida de los residentes de la Comunidad de Madrid
desde 1986 hasta 2023 , comprobando si existen diferencias entre hombres y
mujeres

Alcance.......................................................................................................................
La investigación se limita a los residentes de la Comunidad de Madrid, utilizando
como muestra los datos anuales de edad media de esperanza de vida registrados
desde 1986 hasta 2023

Metodología
Origen de los datos
Se han obtenido los datos del archivo evolucion-de-la-esperanza-de-vida-al-nacer-
por-sexo.csv obtenidos de los datos abiertos de la comunidad de Madrid Catálogo
de Datos Abiertos. (s/f). Comunidad.madrid. Recuperado el 20 de octubre de 2025,
de https://datos.comunidad.madrid/catalogos/#/dataset/602026?view=info que
incluye los valores de la evolución de la esperanza de vida al nacer de mujeres,
hombres y el total desde 1986 hasta 2023.

Herramientas..............................................................................................................
Los datos han sido procesados utilizando el software R y el entorno de desarrollo
Rstudio para Windows en su versión 2025.09.1. Para el cálculo de la moda se
empleó el paquete “ modeest ” y para el cálculo de los coeficientes de asimetría y
apuntamiento se utilizó el paquete “ e1071 ”.

Diseño
Variables Estadísticas:
o Se ha analizado la variable estadística “Edad media”, que representa
la esperanza de vida al nacer de hombres y mujeres obtenidas de los
residentes de la Comunidad de Madrid desde 1986 hasta 2023, de tipo
cuantitativa continua con valores positivos mayores o iguales a 0
o Se ha analizado también la variable estadística “Sexo”. De tipo
cualitativo con los siguientes valores:
▪ “Evolucion de la esperanza de vida al nacer de las mujeres”
▪ “Evolucion de la esperanza de vida al nacer de los hombres”
Población: La población la constituyen el total de residentes en la
Comunidad de Madrid, en los respectivos años.
Muestra: Esta compuesta por los valores anuales de la esperanza de vida al
nacer de hombres y mujeres registrados en la Comunidad de Madrid desde
1986 hasta 2023 con un total de 76 muestras, con 38 en cada grupo.
Organización de datos: Se han eliminado del archivo “ evolucion-de-la-
esperanza-de-vida-al-nacer-por-sexo.csv ” los datos que no se han
utilizado ( Evolución de la esperanza de vida al nacer total ) pasando a tener
un total de 76 observaciones válidas, y las columnas “Código territorio”,
“Territorio”, “Estado dato” con filas vacías. Se ha modificado el archivo
cambiando el nombre de la columna “Concepto” => “Sexo”, y la columna
“Valor” => “Edad_media”, dentro de esta columna se han modificado los “.” a
“,” en los valore, así como la columna “Año” => “Ano”, “Tipo territorio” =>
“Tipo_Territorio”, y “Evolución...” se ha modificado sin acento a “Evolucion...”
para evitar conflictos con los caracteres especiales.
Resultados
Medidas estadísticas
En la tabla 1 se muestran los resultados de las medidas estadísticas de
centralización, dispersión, localización y formas más relevantes, para el total de
datos de la muestra, y para los hombres y las mujeres
Tabla 1. Medidas estadísticas descriptivas
Medida Todos Evolución de la
esperanza de vida al
nacer de las mujeres

Evolución de la
esperanza de vida al
nacer de los hombres
Tamaño muestra 76 datos 38 datos 38 datos
Medidas de centralización

Media 80,93 años 83,97 años 77,88 años
Mediana 81,16 años 84,68 años 78,26 años
Medidas de dispersión

Mínimo 73,15 años 80,19 años 73,15 años
Máximo 87,50 años 87,50 años 82,93 años
Rango 14,35 años 7,31 años 9,78 años
Varianza 18,
años²

6,83 años² 10,84 años²
Desviación estándar 4,25 años 2,61 años 3,29 años
Coeficiente de
variación

0,05 0,03 0,
Medidas de localización

Primer Cuartil (Q1) 78,31 años 81,25 años 74,34 años
Tercer Cuartil(Q3) 84,64 años 86,38 años 81,04 años
Rango intercuartílico 6,33 años 5,12 años 6,70 años
Medidas de forma

Coeficiente de
asimetría

- 0,27 - 0,18 - 0,
Coeficiente de
apuntamiento(curtosis)

- 0,94 - 1,65 - 1,
Otras

Valores inferiores a la
media

35 (46%) 16 (42%) 18 (47%)
Valores superiores a
la media

41 (54%) 22 (58%) 20 (53%)
Tablas de contingencia
En la tabla 2 se muestra la tabla de contingencia para las variables Edad_media y
Sexo, en el caso de agrupar la edad_media en 8 intervalos. En la tabla se
representa con f las frecuencias absolutas y con h las frecuencias relativas.

Tabla 2. Tabla de contingencia para Edad_media y Sexo (con 8 intervalos)
Edad_media/Sexo Evolucion de la
esperanza de vida
al nacer de las
mujeres
Evolucion de la
esperanza de
vida al nacer de
los hombres
fEdad_media hEdad_media
[72,74) 0 8 8 0,
[74,76) 0 5 5 0,
[76,78) 0 5 5 0,
[78,80) 0 7 7 0,
[80,82) 12 9 21 0,
[82,84) 4 4 8 0,
[84,86) 9 0 9 0,
[86,88) 13 0 13 0,
fSexo 38 38 76
hSexo 0,5 0,5 1
En la tabla 3 se muestra una tabla de contingencia para las variables Edad_media y
Sexo en 3 intervalos, diferenciando la la esperanza de vida al nacer en Baja (
Edad_media entre 73 y 77 años), Media (Edad_media entre 77 y 82 años) y Alta
(Edad_media entre 82 y 88 años)

Tabla 3. Tabla de contingencia para Edad_Media y Sexo (Con 3 intervalos)
Edad_medi
a/Sexo
Evolucion de la
esperanza de vida al
nacer de las mujeres
Evolucion de la
esperanza de vida al
nacer de los hombres
fEdad
_medi
a
hEdad
_medi
a
[73,77)
Baja
0 16 16 0,
[77,82)
Media
12 18 30 0,
[82,88) Alta 26 4 30 0,
fSexo 38 38 76
hSexo 0,5 0,5 1
Diagramas
En la figura se muestra el porcentaje de datos por sexo, el número total de datos es

Figura 1. Diagrama con el porcentaje de datos por grupo.
En la figura 2 se muestran los porcentajes de esperanza de vida según su
esperanza de vida baja [73,77), media [77, 82 ) y alta [82,88)

Figura 2. Diagramas de la evolución de la esperanza de vida al nacer
En la figura 3 se muestran los histogramas y diagramas de caja (boxplot) de la
variable edad media, en el caso de los histogramas, agrupada en ocho intervalos,
considerando la edad media total (izquierda), la edad media de las mujeres (centro)
y la edad media de los hombres (derechas). En los diagramas aparecen tanto la
mediana (línea negra continua), como la media (línea roja discontinua)

Figura 3. Histograma y diagramas de caja de la edad media según el sexo
Análisis de resultados
Hay un reparto equitativo de datos entre ambos grupos como se muestra en la
figura 1 y se indica en la tabla 1 un 50% de los 76 datos corresponden a la evolución
de la esperanza de vida de las mujeres (38 muestras) y el otro 50% a los hombres
(38 muestras).

De los datos obtenidos en el histograma (tabla 1) y del boxplot (figura 3) puede
comprobarse que tanto la media como la mediana son mayores en el grupo de
mujeres, donde la media y mediana es 83,97 años y 84,68 años respectivamente,
mientras que en la de los hombres es 77,88 años y 78,26 años.

En ambos casos la mediana es superior a la media, indicando una asimetría
negativa, que indica que existen más valores menores a la media, lo cual se
confirma con el coeficiente de asimetría, que es negativo tanto en mujeres (-0,18)
como en hombres (-0,07), mostrando una asimetría hacia la izquierda, como se
puede apreciar en los histogramas de la Figura 3. De los datos totales recogidos el

46% de los valores está por debajo de la media y el 54% por encima, concretamente
en mujeres el 42% está por debajo y el 58% por encima, y en cambio con los
hombres el 47% está por debajo y el 53% por encima. Se puede observar que el
rango en el caso de las mujeres es de 7,31 años siendo este menor que en el caso
de los hombres que es de 9,78 años.

La desviación estándar del grupo de mujeres es de 2,61 años a comparación con el
de los hombres 3,29 años, esto se refleja también con el coeficiente de variación,
que es 0,03 en mujeres y 0,04 en hombres lo que indica que las esperanzas de vida
de las mujeres varían menos. La mayor dispersión del grupo masculino también se
puede comprobar en los diagramas de caja (Figura 3), donde los bigotes son más
largos y se aprecia una distribución más extendida.

A la vista del diagrama de caja, y por los valores del primer y tercer cuartil en la
Tabla 1, se observa que la mitad de los valores femeninos se sitúa entre 81,25 y
86,38 años, con un rango intercuartílico de 5,12 años, mientras que la mitad de los
valores masculinos está entre 74,34 y 81,04 años, con un rango intercuartílico de
6,70 años, por lo que hay más dispersión en la de los hombres. La mayor dispersión
con ambos grupos ocurre en los valores bajos y medios, viéndose en el diagrama de
caja que el bigote inferior total es más largo.

Si se observan los valores extremos, se puede apreciar que el valor mínimo de la
esperanza de vida es 73,15 años en hombres y en el total de la muestra, mientras
que el máximo es de 87,50 años en el total y en el de mujeres.

El coeficiente de apuntamiento o curtosis en el grupo total es de -0,94, en mujeres
es de -1,65 y en hombres de -1,58, lo que indica que la distribución de frecuencias
es platicúrtica o aplanada, como se puede apreciar en el histograma (Figura 3).
También se puede observar que no se aprecian valores atípicos, y que no hay
mucha concentración de datos cercanos a la media.

En relación con las categorías de esperanza de vida baja [73,77) años, media
[77,82) años, y alta [82,88) años, como se muestra en la Tabla 3 y la Figura 2, se
observa que la mayoría de los datos de las mujeres se concentra en la categoría
alta (26 de 38 mujeres), mientras que la mayoría de los hombres se agrupa en la
categoría media (18 de 38 hombres). Destaca que ningún valor femenino se
encuentra en la categoría baja, mientras que 16 de 38 hombres (42%) pertenecen a
esta categoría de menor esperanza de vida. Esto confirma nuevamente que la
esperanza de vida es significativamente superior en mujeres y que los hombres
presentan mayor dispersión, especialmente hacia los valores más bajos.

Conclusiones
Según los datos obtenidos y el análisis realizado, puede concluirse que en la
Comunidad de Madrid entre 1986 y 2023, la evolución en la esperanza de vida
difiere según el género, aunque la brecha se ha reducido con el tiempo. Las mujeres
presentan una media y mediana superiores a las de los hombres, concentrándose la
mayoría de sus valores en la categoría “Alta” lo que indica una mayor longevidad y
menor dispersión en los datos.

Por otro lado, la evolución en la esperanza de vida de los hombres ha
experimentado un aumento notable, con un mayor porcentaje de valores en las
categorías “Media” y “Alta”, aunque todavía existe una proporción bastante
significativa en la categoría “Baja”.

Por lo tanto, se confirma que existen diferencias en la evolución de la esperanza de
vida entre hombres y mujeres, aunque estas se han visto reducidas con el tiempo.

Referencias
- Catálogo de Datos Abiertos. (s/f). Comunidad.madrid. Recuperado el 26 de
octubre de 2025, de

https://datos.comunidad.madrid/catalogos/#/dataset/602026?view=info
