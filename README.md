# Análisis de Rendimiento de Cultivos y Factores Ambientales en América Latina 🌽🌧️

Este proyecto analiza el impacto de factores ambientales (lluvias, uso de pesticidas, temperatura) en el rendimiento de cultivos en Argentina, Brasil,Mexico,Perú y Chile. El análisis se realiza utilizando datos históricos y visualizaciones interactivas desarrolladas en Power BI para identificar correlaciones y tendencias que pueden influir en la productividad agrícola en la región.

---

## 🎯 Objetivos del Proyecto

1. **Analizar** el rendimiento de cultivos y su variación a lo largo de los años.
2. **Identificar correlaciones** entre el rendimiento de los cultivos y factores como precipitaciones, uso de pesticidas y temperaturas.
3. **Comparar** el rendimiento de cultivos entre los países seleccionados.
4. **Crear un dashboard interactivo** en Power BI que permita visualizar las relaciones y variaciones de los factores estudiados.

## 📁 Estructura del Proyecto

- **data/**: Contiene los archivos CSV con datos de rendimiento, lluvias, pesticidas y temperatura.
- **scripts/**: Incluye scripts de limpieza y transformación de datos (ETL) en Python.
- **dashboard/**: Archivo Power BI (.pbix) con el dashboard interactivo.
- **notebooks/**: Notebooks Jupyter utilizados para el análisis y generación de reportes.

## 🛠️ Herramientas Utilizadas

- **Python**: Para la limpieza y preparación de datos.
- **Pandas**: Para manipulación de los datasets y cálculo de métricas.
- **Power BI**: Para la creación del dashboard interactivo y visualizaciones de datos.
- **Matplotlib & Seaborn**: Para análisis exploratorio y visualización adicional en los notebooks.

## 📊 Dataset

Los datos fueron obtenidos de [Kaggle](https://www.kaggle.com/datasets/patelris/crop-yield-prediction-dataset) e incluyen:
- **Datos de rendimiento de cultivos**: Producción histórica por país y año.
- **Datos de lluvias**: Precipitaciones anuales promedio por país.
- **Datos de temperatura**: Temperatura anual promedio por país.
- **Datos de uso de pesticidas**: Cantidad de pesticidas utilizada en toneladas.

## 📝 Preparación y Limpieza de Datos

1. **Manejo de Nulos**: Los valores faltantes en las columnas de temperatura y precipitaciones se completaron usando la media anual por país.
2. **Estandarización**: Se homogeneizaron los nombres de columnas y países, eliminando espacios en blanco y usando solo las primeras tres letras del país para una columna `id` única en cada dataset.
3. **Filtrado de Países**: Se limitaron los datos a Argentina, Brasil,Mexico,Peru y Chile para enfocarse en la región de interés.

## 🖥️ Análisis y Visualización

Para cada país:
1. **Correlación entre variables**: Se analizó la correlación entre el rendimiento de cultivos y las variables ambientales.
2. **Análisis de tendencias**: Se observaron variaciones a lo largo de los años en las variables y su impacto en el rendimiento.
3. **Visualización de factores clave**:
   - Lluvias y temperatura vs. rendimiento
   - Uso de pesticidas vs. rendimiento

## 🚀 Resultados

Algunos de los hallazgos clave incluyen:
- **Ausencia de correlación positiva/negativa** entre los factores y el rendimiento de cultivos en distintos países.
- **Tendencias temporales** que muestran el impacto de cambios en el clima en los últimos años en los rendimientos de cultivos.
- **Comparación regional** de factores que destacan las diferencias en prácticas agrícolas y condiciones ambientales.

## 📈 Dashboard en Power BI

El dashboard interactivo en Power BI permite visualizar:
- Rendimiento de cultivos y sus variaciones anuales.
- Comparaciones de uso de pesticidas y precipitaciones entre los países.
- Relaciones entre las variables seleccionadas para facilitar el análisis de correlación.

## 📋 Conclusiones y Siguientes Pasos

1. Rendimiento Promedio por País
Se observó que países como Brasil y México lideran en términos de rendimiento promedio (kg/Ha) a lo largo del tiempo, lo que puede atribuirse a mejores prácticas agrícolas, infraestructura y condiciones climáticas favorables. En contraste, países como Perú presentan rendimientos significativamente menores, sugiriendo áreas de oportunidad para optimizar su producción.
2. Rendimiento por Cultivo
Los cultivos como las papas y la yuca tienen una alta productividad en Brasil y México, mientras que otros como el maíz y los camotes muestran un rendimiento más uniforme entre países. Esto resalta la necesidad de focalizar esfuerzos en cultivos estratégicos por región, optimizando recursos para maximizar su potencial.
3. Factores Climáticos y de Insumos
No se identificó una correlación clara entre la temperatura promedio y el rendimiento agrícola, lo que sugiere que la productividad está más influenciada por otros factores, como las prácticas agrícolas y el manejo de insumos. Asimismo, los pesticidas y otros insumos presentan una correlación baja o incluso negativa con el rendimiento, lo que podría reflejar un uso subóptimo o ineficiente en algunas áreas.
4. Desempeño Temporal y Variabilidad
En los últimos años, se ha mantenido una tendencia estable en los rendimientos promedio por país y cultivo, con una ligera convergencia entre las regiones. Sin embargo, persisten brechas significativas en la productividad entre los países, destacando la necesidad de una mayor inversión en tecnología y capacitación agrícola en las regiones con menor rendimiento.
5. Áreas de Mejora
Optimización del uso de insumos: Identificar mejores prácticas para el uso eficiente de pesticidas y fertilizantes.
Focalización en cultivos clave: Priorizar el desarrollo de cultivos que aporten mayor rendimiento en cada país, mejorando así las cadenas de valor agrícola.
Reducción de brechas regionales: Diseñar políticas que fomenten la transferencia tecnológica y la capacitación agrícola en países con menores rendimientos.

---

## 🧑‍💻 Cómo Ejecutar el Proyecto

1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/tu_usuario/analisis-rendimiento-cultivos.git
2. **Instalar dependencias**
   pip install -r requirements.txt
   
3. **Cargar los datos:** Descargar los archivos de datos en la carpeta data/.
   
4. **Ejecutar el ETL y análisis:** Ejecutar los notebooks en notebooks/.
