
# Proyecto Individual #2 HENRY
## Elaborado por Rosa Carmona
### Mayo de 2024

## Análisis Exploratorio de Datos (EDA) sobre Siniestros Viales en Buenos Aires (2016-2021)
### Introducción
Este informe presenta un Análisis Exploratorio de Datos (EDA) sobre una base de datos de siniestros viales con víctimas fatales en la Ciudad Autónoma de Buenos Aires desde 2016 hasta 2021. El análisis proporciona una visión general de los datos, destacando patrones y hallazgos clave, con un enfoque particular en la distribución espacial mediante diversos mapas y filtros que describen perfiles de víctimas y periodos de tiempo. 

#### 1. Preparación y Limpieza del Dataset
###### 1.1 Carga del Dataset

La base de datos se obtuvo del archivo homicidios.xlsx, que incluye información sobre los incidentes (homicidios_raw) y las víctimas (victimas_raw).
La exploración inicial incluyó la verificación de nombres de columnas, tipos de datos y valores faltantes.
1.2 Limpieza de Datos

Los campos temporales (por ejemplo, fechas y horas) se convirtieron a formatos apropiados.
Las coordenadas geográficas se limpiaron y convirtieron a tipos numéricos.
Se identificaron y trataron los valores faltantes según corresponda.
Hallazgos:

Los campos geográficos clave (pos x, pos y) tenían muy pocos valores faltantes (~0.4%).
Los campos relacionados con direcciones tenían una cantidad significativa de datos faltantes, indicando una información incompleta en muchos registros.
1.3 Manejo de Valores Faltantes

Se contaron y abordaron los valores faltantes, enfocándose especialmente en los campos no relacionados con direcciones para mantener la integridad de los datos.
2. Estadísticas Descriptivas de Variables Numéricas
2.1 Valores Máximos y Mínimos

Los incidentes anuales alcanzaron su pico en 2018 con 142 incidentes y disminuyeron a un mínimo en 2020 con 78 incidentes.
Diciembre fue el mes con mayor cantidad de incidentes (77), mientras que septiembre tuvo la menor cantidad (47).
Los patrones semanales mostraron poca variación, con un ligero aumento los lunes (106 incidentes) y una ligera disminución los jueves (94 incidentes).
Los incidentes por hora alcanzaron su pico entre las 5 am y las 7 am, siendo las 6 am la hora con mayor cantidad de incidentes (40) y las 2 am la hora con menor cantidad (17).
2.2 Estadísticas Resumidas

Las estadísticas descriptivas proporcionaron información sobre la distribución de incidentes a lo largo de años, meses, semanas y horas.
Visualización:

Se generaron histogramas y gráficos de barras para ilustrar la distribución temporal de los incidentes.
Las gráficas mostraron que los incidentes anuales variaron significativamente con un aumento en 2018 y una notable disminución en 2020, posiblemente debido a restricciones de movilidad por la pandemia de COVID-19.
La distribución mensual y horaria mostró patrones claros, con un aumento en diciembre y en las primeras horas de la mañana, lo que podría estar relacionado con condiciones de tráfico y visibilidad.
3. Distribución Espacial de los Incidentes
3.1 Mapas de Distribución de Incidentes

Se generaron mapas utilizando folium para visualizar las ubicaciones de los incidentes basados en coordenadas.
Un mapa de calor destacó las áreas con alta concentración de incidentes.
Hallazgos:

Se identificaron altas concentraciones de incidentes en áreas como Liniers, Flores, Constitución y Balvanera.
Estos puntos críticos podrían estar relacionados con áreas de alto tráfico y cruces peligrosos, sugiriendo la necesidad de intervenciones en seguridad vial en estos lugares.
3.2 Análisis por Tipos de Calles

Se crearon tablas de frecuencia para los tipos de calles y nombres de calles específicas con altos incidentes.
Un análisis de Pareto mostró que un pequeño número de calles representaba una porción significativa de los incidentes.
Visualización:

La mayoría de los incidentes ocurrieron en avenidas, seguidas por calles y autopistas.
Calles específicas como "PAZ, GRAL. AV." y "RIVADAVIA AV." presentaron un número notablemente alto de incidentes, lo que indica la necesidad de medidas específicas en estas vías.
4. Análisis por Tipos de Involucrados
4.1 Frecuencias de Víctimas y Acusados

Se analizaron las distribuciones de frecuencia para los tipos de víctimas, acusados y participantes en los incidentes.
Los motociclistas y peatones fueron las víctimas más comunes, mientras que los ocupantes de vehículos privados y transportes públicos fueron a menudo los acusados.
4.2 Exploración del Perfil de las Víctimas

Se realizó un análisis detallado de los perfiles de las víctimas, incluyendo edad, género y rol (por ejemplo, conductor, pasajero).
Las gráficas mostraron que la mayoría de las víctimas eran hombres entre 20 y 40 años, principalmente motociclistas y peatones.
La distribución de edades mostró que las víctimas masculinas tenían un rango más amplio, con algunos outliers mayores de 83 años, mientras que las víctimas femeninas tenían un rango de edades más centrado.
Hallazgos:

La mayoría de las víctimas masculinas eran jóvenes adultos, mientras que las víctimas femeninas tenían una distribución de edad más variada.
Los datos sugieren que las intervenciones de seguridad vial deberían enfocarse en motociclistas y peatones, especialmente en jóvenes adultos.
Conclusión
Este EDA revela hallazgos críticos sobre los patrones y distribuciones de siniestros viales fatales en Buenos Aires desde 2016 hasta 2021. El análisis enfatiza la importancia de los factores espaciales y temporales, así como los perfiles de los involucrados. Estos hallazgos pueden informar intervenciones dirigidas y la formulación de políticas para mejorar la seguridad vial.
