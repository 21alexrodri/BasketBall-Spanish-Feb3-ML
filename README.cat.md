# 🏀 Basketball Player Clustering (K-Means)

Aquest projecte aplica **aprenentatge automàtic no supervisat (K-Means clustering)** per analitzar estadístiques de jugadors de bàsquet i identificar **diferents perfils de joc** segons el seu estil.

Tot l’anàlisi es troba dins **un únic Jupyter Notebook**, on es desenvolupa tot el procés pas a pas.

🌍 Llegir en:
- [English](README.md)
- [Español](README.es.md)
- [Català](README.cat.md)

---

## 📌 Descripció del projecte

Utilitzant estadístiques reals de partits de la Federació Espanyola de Bàsquet (FEB), aquest projecte té com a objectiu:

- analitzar el rendiment dels jugadors  
- extreure variables rellevants des del punt de vista esportiu  
- agrupar jugadors amb estils de joc similars  
- interpretar cada grup des d’una perspectiva baloncestística  

L’objectiu no és predir resultats, sinó **entendre els diferents rols dels jugadors a partir de les dades**.

---

## 🧠 Perfils de jugador identificats

El procés de *clustering* permet identificar **quatre perfils principals de jugador**:

| Cluster | Descripció |
|-------|-------------|
| 0 | Aleros / anotadors ofensius |
| 1 | Jugadors de rotació amb baixa participació |
| 2 | Bases / creadors de joc |
| 3 | Interiors dominants |

Cada clúster s’interpreta a partir de les mitjanes estadístiques i d’exemples reals de jugadors.

---

## 📊 Variables utilitzades

El model final de *clustering* utilitza les següents variables:

- Punts per partit (`pts`)
- Rebots totals (`trb`)
- Pèrdues de pilota (`tov`)
- Ús del tir de 2 punts (`usage_2p`)
- Ús del tir de 3 punts (`usage_3p`)
- Llançaments a la pintura (`paint_shots`)
- Llançaments exteriors (`outside_shots`)
- Ràtio assistències/pèrdues (`ast_tov_ratio`)
- Impacte defensiu (`defensive_impact`)

Totes les variables són estandarditzades abans d’aplicar K-Means.

---

## 📈 Metodologia

El notebook segueix els següents passos principals:

1. Extracció de dades des de MongoDB  
2. Neteja i preprocessament de dades  
3. Enginyeria de variables  
4. Anàlisi exploratòria  
5. Selecció de variables  
6. Escalat de dades  
7. Aplicació de K-Means  
8. Selecció del nombre òptim de clústers (mètodes del colze i de la silueta)  
9. Interpretació dels clústers  
10. Visualització mitjançant PCA  

---

## ⚙️ Tecnologies utilitzades

- Python  
- Pandas 
- Scikit-learn  
- Matplotlib  
- Seaborn  
- MongoDB  
- Jupyter Notebook  

---
