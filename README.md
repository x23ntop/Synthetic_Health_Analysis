# Synthetic_Health_Analysis
Análisis de riesgos de salud

Este repositorio contiene el código y análisis del dataset de salud sintético, incluyendo limpieza, transformación de datos, creación de variables derivadas y visualizaciones. Se ejecuto Python mediante Jupyter Notebooks en Visual Studio Code. Todo código utilizado fue escrito por ChatGPT. 
📌 Contenido

    Análisis exploratorio y limpieza de datos

        Corrección de formato en el archivo CSV.

        Manejo de valores NaN y unknown.

        Conversión de tipos de datos.

        Tratamiento de valores atípicos.

        Creación de variables derivadas.

        Ajuste de variables de tensión arterial.

    Análisis de patrones y visualizaciones

        Relación entre edad, género, sede y nivel de riesgo.

        Asociación entre actividad física, días perdidos y riesgo.

        Gráficos de riesgo por sede y género.

    Estructura del repositorio

    /Synthetic_Health_Analysis/
    ├── README.md
    ├── 2README.ipynb
    ├── Synthetic_dataset.ipynb
    ├── Synthetic_dataset_Complete.ipynb
    ├── corrected_synthetic_data.csv
    ├── synthetic_health_data.csv

📊 Visualizaciones

Ejemplo de gráficos:

import matplotlib.pyplot as plt
import seaborn as sns

plt.figure(figsize=(10,6))
sns.countplot(data=df, x='Sede', hue='Riesgo_Salud_Global', palette='coolwarm')
plt.title('Riesgo global de salud por sede')
plt.xlabel('Sede')
plt.ylabel('Cantidad')
plt.legend(title='Riesgo Salud Global')
plt.show()

plt.figure(figsize=(10,6))
sns.countplot(data=df, x='Genero', hue='Riesgo_Salud_Global', palette='viridis')
plt.title('Riesgo global de salud por género')
plt.xlabel('Género')
plt.ylabel('Cantidad')
plt.legend(title='Riesgo Salud Global')
plt.show()

📜 Licencia

Este proyecto es de uso privado y de análisis de datos.
