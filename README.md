#  Análisis de Uso de Dispositivos Móviles y Comportamiento del Usuario
📊 Resumen del Proyecto
Este repositorio contiene un análisis exploratorio de datos (EDA) y una segmentación de usuarios basada en métricas de uso de dispositivos móviles. El objetivo principal es identificar patrones de comportamiento digital y determinar qué variables son las más predictivas para clasificar a los usuarios en distintos grupos.

El análisis reveló que el género y la edad son factores poco determinantes, mientras que la intensidad de uso (tiempo de pantalla, uso de apps, consumo de batería y datos) permite una segmentación altamente efectiva en 5 clases de usuarios bien definidas.

🔍 Hallazgos Clave del Análisis
Correlaciones Fuertes: Se encontró una correlación lineal y positiva muy marcada entre:

App Usage Time (Tiempo de uso de apps) y Battery Drain (Consumo de batería).

Screen On Time (Tiempo de pantalla encendida) y Battery Drain.

Esto confirma que la intensidad de uso es un factor coherente en todo el dispositivo.

Segmentación por Comportamiento (5 Clases): Las distribuciones de las métricas principales (App Usage, Screen On Time, Battery Drain, Data Usage, Number of Apps Installed) muestran agrupamientos distintos que se alinean perfectamente con la variable User Behavior Class (Clases 1 a 5).

Clase 1 (Ligeros): Bajísimo uso en todas las métricas.

Clase 5 (Muy Intensivos): Uso extremadamente alto y consistente en todas las métricas.

Las clases intermedias (2, 3, 4) representan una progresión lineal en la intensidad del uso.

Irrelevancia Demográfica:

El Género no presenta diferencias significativas en ninguna métrica.

La Edad se distribuye de manera uniforme a través de las 5 clases de comportamiento.

Conclusión: La segmentación debe basarse en hábitos digitales (comportamiento) y no en datos demográficos tradicionales.

🛠️ Tecnologías y Librerías
Python

Pandas: Manipulación y limpieza de datos.

NumPy: Soporte para operaciones numéricas.

Matplotlib & Seaborn: Visualización estática (Boxplots, Histogramas, Gráficos de barras).

Plotly Express: Visualización interactiva (Radar Chart).

scipy.stats: Cálculo de asimetría y curtosis.

📂 Estructura del Repositorio
El corazón del proyecto reside en el notebook de Colab:

[Nombre_del_Colab_o_similiar].ipynb: Contiene la carga de datos, la limpieza, el resumen estadístico y todo el análisis exploratorio y visual.

🚀 Cómo Ejecutar el Análisis
Puedes replicar el análisis siguiendo estos pasos:

Abre el Notebook: Haz clic en el archivo .ipynb para abrirlo directamente en Google Colab.

Ejecuta las Celdas: Ejecuta todas las celdas del notebook de forma secuencial.

Visualiza los Resultados: El notebook generará todos los gráficos estáticos (seaborn/matplotlib) e interactivos (Plotly) que ilustran los hallazgos.

Nota: El dataset se carga directamente desde Google Drive usando un file_id, lo que garantiza que el notebook se ejecute sin problemas de dependencias de archivos locales.
