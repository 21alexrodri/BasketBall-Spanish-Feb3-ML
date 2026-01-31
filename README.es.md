# 🏀 Basketball Player Clustering (K-Means)

Este proyecto aplica **aprendizaje automático no supervisado (K-Means clustering)** para analizar estadísticas de jugadores de baloncesto e identificar **diferentes perfiles de juego** en función de su estilo.

Todo el análisis se encuentra en **un único Jupyter Notebook**, donde el proceso completo se desarrolla paso a paso.

🌍 Leer en:
- [English](README.md)
- [Español](README.es.md)
- [Català](README.cat.md)

---

## 📌 Descripción del proyecto

Utilizando estadísticas reales de partidos de la Federación Española de Baloncesto (FEB), este proyecto tiene como objetivo:

- analizar el rendimiento de los jugadores  
- extraer variables relevantes desde el punto de vista deportivo  
- agrupar jugadores con estilos de juego similares  
- interpretar cada grupo desde una perspectiva baloncestística  

El objetivo no es predecir resultados, sino **comprender los distintos roles de los jugadores a partir de los datos**.

---

## 🧠 Perfiles de jugador identificados

El proceso de *clustering* permite identificar **cuatro perfiles principales de jugador**:

| Cluster | Descripción |
|-------|-------------|
| 0 | Aleros / anotadores ofensivos |
| 1 | Jugadores de rotación con baja participación |
| 2 | Bases / creadores de juego |
| 3 | Interiores dominantes |

Cada clúster se interpreta a partir de las medias estadísticas y de ejemplos reales de jugadores.

---

## 📊 Variables utilizadas

El modelo final de *clustering* utiliza las siguientes variables:

- Puntos por partido (`pts`)
- Rebotes totales (`trb`)
- Pérdidas de balón (`tov`)
- Uso de tiro de 2 puntos (`usage_2p`)
- Uso de tiro de 3 puntos (`usage_3p`)
- Lanzamientos en la pintura (`paint_shots`)
- Lanzamientos exteriores (`outside_shots`)
- Ratio asistencias/pérdidas (`ast_tov_ratio`)
- Impacto defensivo (`defensive_impact`)

Todas las variables son estandarizadas antes de aplicar K-Means.

---

## 📈 Metodología

El notebook sigue los siguientes pasos principales:

1. Extracción de datos desde MongoDB  
2. Limpieza y preprocesamiento de datos  
3. Ingeniería de variables  
4. Análisis exploratorio  
5. Selección de variables  
6. Escalado de datos  
7. Aplicación de K-Means  
8. Selección del número óptimo de clústers (métodos del codo y silueta)  
9. Interpretación de los clústers  
10. Visualización mediante PCA  

---

## ⚙️ Tecnologías utilizadas

- Python  
- Pandas 
- Scikit-learn  
- Matplotlib  
- Seaborn  
- MongoDB  
- Jupyter Notebook  

---
