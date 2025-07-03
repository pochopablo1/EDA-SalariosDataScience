# EDA-SalariosDataScience

Descripción del proyecto
Este proyecto consiste en un Análisis Exploratorio de Datos (EDA) sobre un conjunto de datos de salarios de profesionales en el campo de la Ciencia de Datos, abarcando el período de 2020 a 2023. El objetivo es identificar tendencias, patrones y relaciones entre distintas variables como el nivel de experiencia, la ubicación, el tamaño de la empresa y la modalidad de trabajo, y cómo estas influyen en la remuneración.

📊 conjunto de datos
El dataset utilizado es ds_salaries.csv, el cual contiene información recopilada a través de encuestas a profesionales del sector. Las variables principales incluyen:

work_year: Año en que se registró el salario.

experience_level: Nivel de experiencia (Entry-level, Mid-level, Senior, Executive).

employment_type: Tipo de contrato (Full-time, Part-time, etc.).

job_title: Título del puesto.

salary_in_usd: Salario anual en dólares estadounidenses.

employee_residence: País de residencia del empleado.

remote_ratio: Proporción de trabajo remoto.

company_location: País de ubicación de la empresa.

company_size: Tamaño de la empresa (Pequeña, Mediana, Grande).

⚙️ análisis realizado
El análisis se estructuró en los siguientes pasos:

Limpieza y preprocesamiento de datos:

Eliminación de columnas irrelevantes (salary, salary_currency).

Renombrar códigos de países a sus nombres completos para mayor claridad.

Creación de nuevas variables, como mismo_pais, para comparar la residencia del empleado con la ubicación de la empresa.

Análisis de outliers:

Identificación y visualización de valores atípicos en la variable salary_in_usd para entender su impacto en la distribución.

Análisis de variables univariado y bivariado:

Estudio detallado de la distribución y tendencias de cada variable clave.

Análisis de la evolución de los salarios a lo largo de los años y su relación con el nivel de experiencia, tipo de empleo, y tamaño y ubicación de la empresa.

Análisis de correlación:

Uso de la correlación de Spearman para medir la fuerza y dirección de la relación entre las variables, especialmente enfocándose en los factores que influyen en el salario.

Test de hipótesis:

Aplicación del test U de Mann-Whitney para validar estadísticamente si existen diferencias significativas en las medianas salariales entre diferentes años y si la proporción de trabajo remoto ha cambiado a lo largo del tiempo.

🚀 conclusiones principales
Tendencia salarial al alza: Se confirma una tendencia positiva en los salarios del sector, con un crecimiento estadísticamente significativo entre 2021 y 2023.

La experiencia es clave: El nivel de experiencia es el predictor más fuerte del salario. Los roles de nivel Executive y Senior reciben las remuneraciones más altas.

Dominio geográfico de EE. UU.: Estados Unidos lidera el mercado tanto en número de empleos como en los salarios más competitivos.

Impacto del trabajo remoto: Contrario a la creencia popular, el porcentaje de trabajos totalmente remotos no ha aumentado de forma constante, mostrando incluso una disminución en 2023. Los salarios para puestos totalmente remotos son ligeramente superiores a los presenciales, pero la diferencia no es drástica.

🛠️ tecnologías utilizadas
Python 3

Pandas: Para la manipulación y análisis de datos.

NumPy: Para cálculos numéricos.

Matplotlib y Seaborn: Para la visualización de datos.

Plotly: Para gráficos interactivos.

SciPy: Para pruebas estadísticas (Shapiro, Mann-Whitney U).

Scikit-learn: Para la codificación de variables categóricas.

