Análisis Exploratorio de Churn de Clientes – Telecom X

--- Descripción del Proyecto ---

Este proyecto aborda el problema de evasión de clientes (Churn) en Telecom X, una empresa de telecomunicaciones que enfrenta una tasa significativa de cancelaciones.

El objetivo del análisis es comprender los factores asociados al abandono de clientes, a partir del procesamiento, limpieza y exploración de los datos, generando insights que permitan al equipo de Data Science avanzar hacia modelos predictivos y estrategias de retención más efectivas.


--- Objetivo del Análisis ---

- Analizar la distribución y magnitud del churn en la base de clientes.

- Identificar patrones asociados a la antigüedad, tipo de contrato, método de pago y cargos.

- Explorar relaciones entre variables clave mediante análisis descriptivo y correlacional.

- Proveer conclusiones accionables que contribuyan a reducir la evasión de clientes.


--- Dataset ---

- Fuente:
https://raw.githubusercontent.com/alura-cursos/challenge2-data-science-LATAM/main/TelecomX_Data.json

- Descripción general del dataset:

7.267 registros de clientes

Variables categóricas y numéricas

Variable objetivo: Churn (Abandono)

- Variables clave analizadas:

Antigüedad del cliente (Meses_antiguedad)

Tipo de contrato

Método de pago

Cargo mensual

Cargo total

Cuenta diaria (variable derivada)



--- Metodología de Análisis ---

El análisis se desarrolló siguiendo las siguientes etapas:

- Carga e inspección inicial del dataset

- Revisión de tipos de datos

- Identificación de valores faltantes y formatos inconsistentes

- Limpieza y tratamiento de datos

- Normalización de valores vacíos en Cargo_total

- Conversión de variables categóricas (Yes / No) a formato numérico

- Renombrado de columnas para mayor claridad

- Creación de la variable derivada Cuentas_Diarias

- Análisis Exploratorio de Datos (EDA)

- Distribución general del churn


- Análisis del abandono según:

Antigüedad del cliente

Tipo de contrato

Tipo de servicio de internet


- Visualizaciones con Matplotlib y Seaborn

- Análisis de correlaciones

- Evaluación de relaciones entre variables numéricas

- Identificación de factores con mayor asociación al abandono



--- Principales Hallazgos ---

- Aproximadamente el 25–28% de los clientes abandonan el servicio, lo que evidencia un problema relevante de churn.

- La tasa de abandono es significativamente mayor en los primeros meses de relación, disminuyendo progresivamente a medida que aumenta la antigüedad del cliente.

- Los clientes con contratos Month-to-month presentan una tasa de churn muy superior a aquellos con contratos anuales o de dos años.

- El servicio de fibra óptica registra la mayor tasa de abandono en comparación con DSL o clientes sin servicio de internet.

- El análisis de correlación mostró una relación negativa moderada entre antigüedad y abandono, reforzando la importancia del ciclo de vida del cliente.



--- Conclusiones e Insights ----

El análisis exploratorio permitió identificar que el churn se concentra principalmente en:

Clientes con baja antigüedad

Contratos mensuales

Usuarios del servicio de fibra óptica

Estos patrones sugieren que tanto la experiencia inicial del cliente como la estabilidad contractual juegan un rol fundamental en la retención. Asimismo, ciertos servicios presentan un riesgo mayor de abandono y requieren una revisión específica.


--- Recomendaciones Estratégicas ---

En base a los resultados obtenidos, se recomienda:

- Implementar estrategias de retención temprana durante los primeros meses del cliente.

- Incentivar la migración de contratos mensuales hacia planes de mayor duración mediante promociones o beneficios.

- Analizar en profundidad el servicio de fibra óptica para detectar posibles problemas técnicos, de calidad o de percepción de valor.

- Utilizar los insights obtenidos como base para el desarrollo de modelos predictivos de churn.


--- Tecnologías Utilizadas ---

- Python

- Pandas

- Matplotlib

- Seaborn

- Jupyter Notebook


--- Cómo Ejecutar el Proyecto ---

1- Clonar el repositorio

2- Instalar las dependencias necesarias

3- Abrir el notebook en Jupyter Notebook o Jupyter Lab


--- Proceso de Aprendizaje y Acompañamiento ---
Me parece importante aclarar que el desarrollo de este proyecto se realizó en un contexto formativo, utilizando un asistente de IA como herramienta de apoyo conceptual y metodológico, no como fuente directa de código ni de soluciones cerradas.

La utilización del asistente IA se enfoco en:

- Orientar el razonamiento analítico y la secuencia lógica del análisis exploratorio

- Sugerir enfoques, preguntas y criterios para interpretar los datos

- Ayudar a identificar buenas prácticas en limpieza, transformación y visualización de datos

- Facilitar la comprensión de conceptos estadísticos y de análisis de datos aplicados al problema de churn

La escritura del código, la elección de visualizaciones, el diseño del flujo del notebook y la interpretación final de los resultados fueron realizados de manera activa, reflexiva y autónoma, recurriendo a la documentación oficial y a mis propios apuntes cuando fue necesario.

Este enfoque permitió que el proyecto funcione como una instancia real de aprendizaje, fortaleciendo la capacidad de análisis, toma de decisiones y comunicación de insights basada en datos.
