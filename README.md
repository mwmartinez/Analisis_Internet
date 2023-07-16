# Analisis de datos sobre las telecomunicaciones en argentina

## Introduccion
En la era digital actual, las telecomunicaciones desempeñan un papel fundamental en la conectividad global, permitiendo la transmisión de información de manera rápida y eficiente. En particular, el internet ha revolucionado la forma en que nos comunicamos y accedemos a la información, y ha generado impactos significativos en diversas áreas de nuestras vidas.

En el caso de Argentina, el desarrollo de las telecomunicaciones ha experimentado un avance notable en los últimos años. Según datos del año 2020, el país cuenta con un impresionante total de 62,12 millones de conexiones, situándose por encima de la media mundial en términos de desarrollo tecnológico.

Este contexto prometedor crea oportunidades emocionantes para mejorar aún más las telecomunicaciones en Argentina y optimizar la conectividad en todo el país. Para lograrlo, es necesario un análisis exhaustivo de los datos relacionados con las telecomunicaciones, que nos permita comprender los desafíos existentes y encontrar soluciones innovadoras.

En este repositorio, presentamos un enfoque de análisis de datos para mejorar las telecomunicaciones en Argentina. Exploraremos diferentes aspectos de este campo, desde la calidad del servicio hasta la infraestructura de red, con el objetivo de identificar áreas de mejora y proponer estrategias efectivas.

Nuestro trabajo se basa en la premisa de que una mejor conectividad y una calidad de servicio óptima en las telecomunicaciones son fundamentales para el desarrollo económico, social y tecnológico del país. Al utilizar técnicas de análisis de datos, buscamos brindar insights valiosos que puedan guiar decisiones informadas para el avance continuo de las telecomunicaciones en Argentina.

## Objetivos
- Analizar la penetración del servicio de internet fijo por cada 100 hogares en cada provincia a lo largo del tiempo.
- Evaluar el acceso al servicio de internet fijo por banda ancha y angosta en cada provincia.
-  Identificar las tecnologías más utilizadas para el acceso al servicio de internet fijo por provincia.
- Analizar la velocidad media de bajada del internet fijo por provincia a lo largo del tiempo.
- Evaluar el acceso al servicio de internet fijo por velocidad en cada provincia.
- Analizar los ingresos trimestrales de los operadores por el servicio de internet.

## Datos
En este proyecto, encontrarás dos carpetas que contienen los conjuntos de datos iniciales. La carpeta [datos](https://github.com/mwmartinez/Analisis_Internet/tree/main/datos) contiene los conjuntos de datos originales, mientras que la carpeta datos_limpios alberga los conjuntos de datos después de haber pasado por el proceso de Extracción, Transformación y Carga (ETL).

La carpeta de datos es el punto de partida, donde podrás explorar los conjuntos de datos tal como se obtuvieron inicialmente. Estos datos pueden requerir un procesamiento adicional antes de poder utilizarlos en el análisis.

Por otro lado, la carpeta de [datos_limpios](https://github.com/mwmartinez/Analisis_Internet/tree/main/datos_limpios) contiene los conjuntos de datos procesados y listos para su análisis. Durante el proceso de ETL, se realizaron diversas transformaciones, como la limpieza de datos erróneos o incompletos, la normalización de formatos y la integración de diferentes fuentes de datos. Esto garantiza que los conjuntos de datos estén en un estado óptimo para su uso en el análisis de telecomunicaciones en Argentina.

## Analis Exploratorio De Datos
Para realizar el EDA se utilizó Python con librerías de Numpy, Pandas, Matplotlib y Seaborn, entre otras. Se pueden visualizar las transformaciones y los análisis realizados en el siguiente archivo [eda](https://github.com/mwmartinez/Analisis_Internet/blob/main/eda.ipynb)

## Importacion a power bi y modelado de datos
se realizo el siguiente modelo de datos ![Logo](https://github.com/mwmartinez/Analisis_Internet/blob/main/src/modelo.png)


El modelo de datos para el análisis de las telecomunicaciones en Argentina se compone de varios conjuntos de datos, cada uno proporcionando información relevante sobre diferentes aspectos de la conectividad y los servicios de internet. A continuación, se describen brevemente los datos disponibles y las columnas que los componen:

internet_penetracion: Este conjunto de datos presenta la penetración de internet fijo en cada provincia, representada como el número de accesos al servicio de internet fijo por cada 100 hogares. Las columnas incluidas son: 'Año', 'Trimestre', 'Provincia' y 'AccesoX100Hog'.

internet_baf_1: Este conjunto de datos ofrece información sobre los accesos al servicio de internet fijo por banda ancha y banda angosta en cada provincia. Las columnas incluyen: 'Año', 'Trimestre', 'Provincia', 'Banda ancha fija', 'Dial up' y 'Total'.

Internet_Accesos-por-tecnologia: Este conjunto de datos muestra el número de accesos al servicio de internet fijo desglosados por tecnología utilizada en cada provincia y trimestre. Las columnas son: 'Año', 'Trimestre', 'Provincia', 'ADSL', 'Cablemodem', 'Fibra óptica', 'Wireless', 'Otros' y 'Total'.

historico_velocidad: Este conjunto de datos proporciona la velocidad media de bajada del internet fijo en cada provincia. Las columnas incluyen: 'Año', 'Trimestre', 'Provincia' y 'Mbps'.

acceso_internet_fijo_por_velocidad: Este conjunto de datos presenta los accesos al servicio de internet fijo clasificados por velocidad en cada provincia y trimestre. Las columnas incluyen: 'Año', 'Trimestre', 'Provincia', 'HASTA 512 kbps', '+ 512 Kbps - 1 Mbps', '+ 1 Mbps - 6 Mbps', '+ 6 Mbps - 10 Mbps', '+ 10 Mbps - 20 Mbps', '+ 20 Mbps - 30 Mbps', '+ 30 Mbps', 'OTROS' y 'Total'.

ingreso_trimestral_operadores: Este conjunto de datos muestra los ingresos trimestrales generados por los operadores de servicios de internet. Las columnas son: 'Año', 'Trimestre', 'Ingresos' y 'Periodo'.

Estos conjuntos de datos proporcionan una visión completa de diversos aspectos de las telecomunicaciones en Argentina, incluyendo la penetración de internet, el acceso por tecnología y velocidad, así como los ingresos generados por los operadores. Al combinar y analizar estos datos, se puede obtener información valiosa sobre el estado y el rendimiento de las telecomunicaciones en el país, lo que puede servir como base para la toma de decisiones estratégicas y la mejora continua de los servicios de internet en Argentina.

## DASHBOARD REALIZADOS

### Accesos 
![Logo](https://github.com/mwmartinez/Analisis_Internet/blob/main/src/accesos.png)

El análisis de la penetración de Internet por provincia en Argentina revela una tendencia general de crecimiento constante a lo largo del tiempo. Se observa un aumento en el número de accesos por cada 100 hogares, indicando una mayor adopción de Internet en la población.

En los últimos años, se ha observado una aceleración en el crecimiento de la penetración de Internet, especialmente a partir de 2018. Esto refleja un incremento significativo en la adopción de Internet en los hogares argentinos.

Sin embargo, existen diferencias marcadas en la penetración de Internet entre las provincias. La Capital Federal destaca con la mayor penetración, con un porcentaje del 113% de accesos por cada 100 hogares, mientras que provincias como Formosa muestran la menor penetración, con solo el 26% de accesos.

Además, se pueden identificar patrones regionales, donde provincias como Buenos Aires, Córdoba, Santa Fe y La Pampa muestran una penetración relativamente alta de Internet, mientras que provincias como Formosa, Santiago del Estero y Chaco presentan una menor penetración.

Este análisis resalta la necesidad de tomar medidas para mejorar la infraestructura y promover la inclusión digital en las provincias con baja penetración de Internet. Además, identifica áreas clave para el desarrollo y la adopción de servicios de Internet, como la Capital Federal y otras provincias con alta penetración.

Utilizando estos datos, se pueden diseñar estrategias de expansión y promoción de servicios de Internet en las provincias con menor acceso, con el objetivo de cerrar la brecha digital y promover la inclusión de más hogares en la era digital en Argentina.

### Conexiones
![Logo](https://github.com/mwmartinez/Analisis_Internet/blob/main/src/conexiones.png)

Al analizar los datos agrupados por año y tecnología, se observa una tendencia general de aumento en el número de accesos a Internet fijo a lo largo de los años. Sin embargo, se pueden identificar algunas diferencias y patrones interesantes:

La tecnología de Cablemodem es la más utilizada y muestra un crecimiento constante a lo largo del tiempo. Es la opción preferida en la mayoría de los años, con un aumento significativo en el número de accesos.

La tecnología de Fibra óptica ha experimentado un crecimiento notable, especialmente a partir de 2019. En 2022, alcanza su punto máximo con una cantidad considerable de accesos, lo que indica una creciente adopción de esta tecnología de alta velocidad.

Por otro lado, la tecnología de ADSL muestra una disminución gradual en el número de accesos, especialmente después de 2018. Esto puede indicar una preferencia de los usuarios por tecnologías más avanzadas y velocidades de conexión más altas.

La tecnología inalámbrica (Wireless) tiene una presencia limitada en comparación con las otras tecnologías, con una cantidad relativamente baja de accesos en todos los años analizados.

En resumen, los datos revelan que en Argentina, las conexiones por Cablemodem y Fibra óptica son las más utilizadas, mientras que las conexiones inalámbricas tienen una presencia menor. Esto indica una preferencia por tecnologías cableadas debido a su mayor rendimiento y confiabilidad.

Estos hallazgos pueden ser útiles para las empresas y proveedores de servicios de Internet en Argentina, ya que les permiten comprender las preferencias y demandas de los usuarios, así como adaptar sus ofertas y estrategias para satisfacer las necesidades de conectividad de la población.


## Velocidad E ingresos
![Logo](https://github.com/mwmartinez/Analisis_Internet/blob/main/src/velocidad.png)

Velocidad de conexión:

La mayoría de los usuarios encuestados (44.9%) tienen velocidades de conexión en el rango de 1 Mbps a 6 Mbps, lo que indica una proporción considerable de usuarios aún con velocidades moderadas.
Las velocidades más bajas representan un porcentaje menor de usuarios, y se observa una disminución gradual en su número.
Se registra un aumento en el número de usuarios con velocidades más altas, especialmente en el rango de 10 Mbps a 30 Mbps.
La categoría "OTROS" representa una proporción baja de usuarios, indicando una pequeña fracción con velocidades de conexión no clasificables fácilmente.
Ingresos trimestrales:

Los ingresos trimestrales muestran un aumento gradual a lo largo de los años, con un patrón estacional.
Los trimestres finales de cada año suelen tener ingresos más altos, posiblemente debido a las festividades y compras navideñas.
El primer trimestre del año tiende a tener ingresos más bajos, probablemente debido a una disminución en el consumo después de las vacaciones.
Se observa un incremento significativo en los ingresos trimestrales en 2022 en comparación con los años anteriores, lo cual puede indicar un aumento en la demanda o en los precios durante ese período.
En general, estos análisis revelan una tendencia positiva hacia velocidades de conexión más altas, con un aumento en la adopción de velocidades de 10 Mbps a 30 Mbps. Sin embargo, todavía hay una proporción considerable de usuarios con velocidades moderadas. En cuanto a los ingresos trimestrales, se observa un crecimiento gradual a lo largo de los años, con variaciones estacionales. El último trimestre destaca por tener ingresos más altos, posiblemente debido a eventos festivos y de compras.

Es importante considerar que estos análisis se basan en los datos proporcionados y pueden requerir un contexto más amplio para una interpretación completa. Además, es recomendable considerar otros factores económicos y del mercado al analizar los ingresos trimestrales.

## conclusiones

onclusiones generales del análisis de datos de telecomunicaciones en Argentina:

Tendencia hacia mayores velocidades de conexión: El análisis de la velocidad de conexión revela una tendencia positiva hacia velocidades más altas, con un aumento en la adopción de velocidades de 10 Mbps a 30 Mbps. Sin embargo, todavía hay una proporción considerable de usuarios con velocidades moderadas, lo que sugiere que existe margen de mejora en términos de velocidad y calidad de conexión.

Disminución de velocidades más bajas: Se observa una disminución gradual en el número de usuarios con velocidades de conexión más bajas, lo que indica una mejora en la infraestructura y una mayor disponibilidad de servicios de Internet de mayor velocidad. Esta disminución es alentadora, ya que demuestra un avance hacia una conectividad más rápida y confiable.

Preferencia por tecnologías por cable: Los datos revelan una preferencia por las tecnologías de Cablemodem y Fibra óptica, que presentan un crecimiento constante a lo largo del tiempo. Esto refleja una elección de los usuarios por conexiones por cable debido a su mayor rendimiento y confiabilidad.

Aumento en los ingresos trimestrales: Los ingresos trimestrales muestran un crecimiento gradual a lo largo de los años, con incrementos significativos en algunos periodos. Esto indica una creciente demanda de servicios de Internet y sugiere un mercado en crecimiento en el sector de las telecomunicaciones en Argentina.

Variaciones estacionales en los ingresos: Se observa una variabilidad estacional en los ingresos trimestrales, con un aumento en el último trimestre del año y una disminución en el primer trimestre. Estas variaciones pueden estar relacionadas con las festividades y las temporadas de compras, lo que indica una influencia de factores estacionales en el consumo de servicios de Internet.

En general, los análisis destacan una evolución positiva en las telecomunicaciones en Argentina, con un aumento en las velocidades de conexión y los ingresos trimestrales. Sin embargo, también señalan áreas de mejora, como la necesidad de seguir impulsando la adopción de velocidades más altas y reducir la brecha digital en regiones con menor penetración de Internet. Estos hallazgos pueden guiar estrategias y políticas orientadas a mejorar la conectividad y promover un acceso equitativo a los servicios de Internet en todo el país.
