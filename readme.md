<p align=center><img src=https://2.bp.blogspot.com/-m8z2JI7CPGY/WlQR8-j36jI/AAAAAAABN9k/FuzPP9hkvxobfktIhhte6PfIoNhYn7NigCLcBGAs/s1600/74179157.jpg width="350"/>


# PROYECTO INDIVIDUAL N°2 - Data Analytics

## *Desarrollado por Carlos Sanchez para La Organización de Aviación Civil Internacional (OACI) * 


#### `Proyecto`:
- **Análisis de Accidentes Aéreos** Este proyecto consiste en analizar una base de datos histórica de accidentes aéreos ocurridos entre 1908 y 2021. El objetivo es identificar patrones, tendencias y factores que puedan mejorar la seguridad en la aviación.

#### Rol del desarrollador:
- Data Analytics

<hr> 

- **Objetivo**

El objetivo principal del proyecto es:

Realizar un análisis de los datos entregados por la OACI de los accidentes aéreos cuyo requerimiento es de vital importancia para identificar áreas de mejora en temas como seguridad, capacitación y diseño de aviones


<hr>

`Entregables`

El proyecto se divide en diferentes etapas y se generaron los siguientes entregables:

 1. **EDA**: este archivo de Analisis Exploratorio de los Datos se subira al repositorio de Github, CASA27: notebook (.ipynb), archivo que contienen  análisis descriptivos de los datos, donde se enocontraran gráficas univariadas y bivariadas para identificar patrones y tendencias. 
[eda.ipynb]( https://github.com/CASA27/Analisis_Datos/blob/master/eda.ipynb)*

2. **Dashboard Interactivo**: archivo .pbix que tendra un dashboard interactivo, para permitir explorar y visualizar los datos de manera dinámica, indicadores, graficas y KPIs (Indicadores Clave de Desempeño) que nuestro cliente ha solicitado, OACI. 
[da.pbix](https://github.com/CASA27/Analisis_Datos/blob/master/da.pbix)*

3. **KPI**: se crearon 3 KPIs mas el solicitado por el cliente, estos KPIs se deben explicar en una reunion con los interesados del proyecto, miembros de la OACI.

4. **Repositorio de Github**: en mi repositorio CASA27 se alojara todo el desarrollo del proyecto para visualizacion del cliente.


  <hr> 


`Archivos y Carpetas`

+ ETL/: Contiene los scripts y archivos relacionados con el proceso de Extracción, Transformación y Carga de los datos.  
[etl.ipynb](https://github.com/CASA27/Analisis_Datos/blob/master/etl.ipynb)*

+ EDA/: Contiene el notebook (.ipynb) con el análisis exploratorio de datos.

+ Dashboard/: Contiene el archivo .pbix con el dashboard interactivo.

+ KPIs/: Contiene información y documentación relacionada con los KPIs generados.

+ Data/: Carpeta que contiene la base de datos histórica de accidentes aéreos.


##### *Nota: Estos archivos y carpetas se encuentra alojados la carpeta [Analisis_Datos](https://github.com/CASA27/Analisis_Datos)*

<hr>


#### Tecnologías utilizadas:
- Visual studio code (Editor de código fuente desarrollado por Microsoft, herramienta de desarrollo)
- Python (Lenguaje de programacion utilizado para los procesos de ETL y EDA)
- Bibliotecas de Python utilizadas (Pandas, matplotlib y Seaborn )
- Power BI Desktop (Para visualización y creación del dashboard interactivo).

<hr>

`Instrucciones de Uso`

A continuación, se detallan las instrucciones para utilizar y acceder a los diferentes componentes del proyecto:

**Proceso EDA**

- Notebook de Análisis Exploratorio de Datos
- Accede a la carpeta EDA/ en el repositorio.
- Abre el archivo del notebook de análisis exploratorio de datos (archivo con extensión .ipynb) utilizando una herramienta compatible con Jupyter Notebook.
- Asegúrate de tener las bibliotecas de Python requeridas instaladas.
- Ejecuta las celdas del notebook secuencialmente para realizar el análisis exploratorio de datos.
- Examina los resultados, gráficos y conclusiones obtenidos a partir del análisis.

**Dashboard Interactivo**
- Ve a la carpeta Dashboard/ en el repositorio.
- Abre el archivo .pbix utilizando Power BI Desktop (asegúrate de tenerlo instalado).
- Dentro de Power BI Desktop, verifica las conexiones y la ubicación de los datos.
- Explora las diferentes visualizaciones, filtros y herramientas interactivas proporcionadas en el dashboard.
- Interactúa con los datos para obtener información relevante y realizar análisis personalizados.
- Guarda el archivo .pbix con cualquier cambio realizado en el dashboard.
- Recuerda que para ejecutar el proceso de EDA y utilizar el notebook de análisis exploratorio de datos, es necesario contar con Python y las bibliotecas mencionadas previamente. Además, para acceder al dashboard interactivo, debes tener instalado Power BI Desktop.

- Si tienes alguna duda o inconveniente durante el uso del proyecto, no dudes en consultar la documentación o contactar al equipo responsable del análisis de accidentes aéreos.


<hr>

**Resultados y Conclusiones**

Con los analisis univariados y bivariados de nuestro EDA, encontramos informacion importante, metricas que nos ayudaron a entender las causas mas frecuentes de los accidentes aereos, tales como;

+ Total de fallecidos historicamente → 111470
+ Total de Sobrevivientes → 43929
+ Mes donde historicamente hay mas accidentes → Diciembre
+ Dia historico donde ocurren as accidentes → dia 8, seguido del dia 15
+ De acuerdo al historico de accidentes desde 1908 hasta 2021 observamos 2 picos donde hubieron mayores accidentes, uno en 1946 con 88 accidentes y otro en 1980 con  83 accidentes, tambien observamos que los años donde hubieron menores accidentes fueron en 1908 con 1 accidente, tiene sentido al iniciar con los archivos o bases de datos en aquella epoca y en 2021 con 7 accidentes
+ Encontramos Aeroflot como el mayor operador donde hubieron accidentes → 8802 Fallecidos 
+ El avion con mas accidentes → Douglas DC-3 con 4725 
+ Tasa de Moratalidad es del 71,77% 
+ Tasa de Supervivencia es del 28,23%
+ Total de muertos por Ruta → La ruta Tenerife, Canary Islands con 761  

**KPIs**

**1.**  Disminucion de la Tasa de Mortalidad en un 5%

Fórmula de medición

TasaMortalidad = DIVIDE(SUM(Aviones[Total Fallecidos]), SUM(Aviones[Total a Bordo])) * 100


**2.** Disminucion del 5% de personas fallecidas en Tierra

Fórmula de medición

KPI Red Fallecidas_Tierra = AVERAGE([Fallecidas en Tierra]) * 0.95


**3.** Reducir en 5% la tasa de mortalidad a nivel anual, siendo el número de fallecidos en los accidentes aéreos respecto al total de personas en los vuelos involucrados.

Fórmula de medición

TasaMortalidad = DIVIDE(SUM(Aviones[Total Fallecidos]), SUM(Aviones[Total a Bordo])) * 100
Tasa_Mortalidad_Red = [TasaMortalidad] * (1 - 0.05)


**4.** Aumentar la Tasa de Supervivencia en un 5%

Fórmula de medición

Tasa de Supervivencia = DIVIDE(SUM(Aviones[Total a Bordo]) - SUM(Aviones[Total Fallecidos]), SUM(Aviones[Total a Bordo])) * 100

`Conclusiones`

**1.** El análisis de los accidentes aéreos puede ayudar a identificar patrones y tendencias que pueden ser utilizados para mejorar la seguridad en la aviación. Esto puede incluir el desarrollo de mejores prácticas, capacitaciones, reentrenamiento, etc.

**2.** Se pueden identificar diversos factores que estan muy relacionados con los accidentes aéreos, como fallas mecánicas, errores humanos, condiciones climáticas adversas, entre otros. Estos factores pueden servir como referencia para implementar medidas de prevención y mitigación.

**3.** El análisis de los datos históricos de accidentes de avión nos muestra una tendencia general de disminución en el número de accidentes a lo largo de los años, especialmente en los ultimos 10 años, esto podria ser por mejoras en la seguridad y en las regulaciones de la aviación a lo largo del tiempo, siendo muy importante La Organización de Aviación Civil Internacional (OACI)






<hr>

<img src="https://visualstudio.microsoft.com/wp-content/uploads/2019/06/vs-code-responsive-01.svg" width="50"/><img src="https://www.python.org/static/community_logos/python-logo.png" width="150"/><<img src="https://media.giphy.com/avatars/OndaFit/yZpY51PVJFaC.png" width="50"/> <img src="https://img2.freepng.es/20180326/eye/kisspng-github-computer-icons-logo-github-5ab8a338143da0.8375508315220498480829.jpg" width="50"/>