# Análisis de Congestión Vehicular vs. PIB per cápita — LATAM

Proyecto de análisis de datos en Python que examina la relación entre la congestión 
vehicular y el PIB per cápita en 14 ciudades de 7 países de América Latina, con el 
objetivo de identificar ciudades prioritarias para inversión en infraestructura de 
transporte.

## Contexto y objetivo

¿Existe una relación entre la movilidad urbana (congestión, tiempos de viaje) y la 
productividad económica (PIB per cápita)? Este análisis integra datos de tráfico y 
economía para responder esa pregunta con evidencia, no solo intuición.

## Datos

- `oecd_city_economy.csv` — Dataset de PIB per cápita por ciudad, incluido en este repositorio.
- `tomtom_traffic` — Dataset de congestión vehicular provisto por TomTom como parte del 
  bootcamp de análisis de datos en TripleTen. No se incluye en este repositorio por su 
  tamaño (~142 MB, supera el límite de GitHub).

## Metodología

- Estandarización de nombres de país entre ambas fuentes (inglés/español, tildes)
- Agregación de datos de tráfico por ciudad-año
- Integración de tráfico y economía mediante join
- Validación visual con boxplot e histogramas antes del análisis de correlación
- Cálculo del coeficiente de correlación de Pearson entre congestión y PIB per cápita

## Hallazgos principales

- El promedio de congestión en LATAM (629.52) es considerablemente más alto que el 
  promedio global del dataset completo (178.14).
- Se observa una relación negativa entre congestión y PIB per cápita: ciudades con 
  mayor congestión tienden a tener menor productividad económica relativa.
- **Bogotá** se identifica como la ciudad con el perfil más claro de alta congestión 
  combinada con baja productividad relativa, siendo la recomendación principal para 
  priorizar inversión en infraestructura de transporte.

## Tecnologías utilizadas

Python (pandas, NumPy, Matplotlib, Seaborn) · Estadística descriptiva · 
Análisis de correlación (Pearson)

## Autora

Johana Farath Salas Pasuy — [LinkedIn](https://www.linkedin.com/in/johana-farath-salas-pasuy-b7907a27)
