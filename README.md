# PHA Predictor — Potentially Hazardous Asteroid

Clasificación binaria de asteroides potencialmente peligrosos (PHA) a partir de variables físicas y de aproximación de la NASA.
Proyecto de aula de **Modelos y Simulación de Sistemas II** — Universidad de Antioquia.

**Integrantes:** Eliana Maria Brand Agudelo, Jilberth Ferney Alzate Castaño, Juan Esteban Gil Quintero.

## Contenido (Entregable I)

| Archivo | Descripción |
|---|---|
| `reporte.pdf` | Informe en plantilla IEEE: descripción del problema y estado del arte. |
| `entregable1.ipynb` | Notebook con las mismas secciones del informe; reproduce todas sus cifras, tablas y figuras. No escribe archivos. |
| `neo.csv` | Datos: [NASA – Nearest Earth Objects](https://www.kaggle.com/datasets/sameepvani/nasa-nearest-earth-objects) (Kaggle, S. Vani; licencia CC0, dominio público). 90 836 filas, 10 variables. |

## Cómo reproducir

1. Instalar las dependencias:
   ```bash
   pip install numpy pandas scipy scikit-learn matplotlib seaborn jupyter
   ```
2. Abrir el notebook desde la carpeta del repositorio (`neo.csv` debe quedar junto a él) y ejecutarlo completo ("Run All"):
   ```bash
   jupyter notebook entregable1.ipynb
   ```
