# Análisis del uso de ConnectaTel

## Descripción del proyecto

Este proyecto analiza los patrones de uso de los clientes de ConnectaTel, una empresa de telecomunicaciones con operaciones en México y Colombia.

El objetivo es identificar patrones de uso, detectar comportamientos atípicos y segmentar a los clientes según su edad y nivel de uso de los servicios de llamadas y mensajes, con el fin de generar información útil para futuras decisiones comerciales.

## Datasets utilizados

El análisis integra tres fuentes de datos:

- `plans.csv`: información de los planes disponibles.
- `users_latam.csv`: información de los usuarios, incluyendo edad, ciudad, plan y fechas de registro y cancelación.
- `usage.csv`: registros de uso de llamadas y mensajes.

## Etapas del análisis

1. Carga y exploración inicial de los datasets.
2. Identificación y tratamiento de valores faltantes, sentinels e inconsistencias.
3. Conversión y validación de tipos de datos.
4. Integración y agregación de información por usuario.
5. Análisis estadístico descriptivo.
6. Visualización de distribuciones mediante histogramas y boxplots.
7. Identificación de valores atípicos mediante el método IQR.
8. Segmentación de usuarios por edad y nivel de uso.
9. Elaboración de insights y recomendaciones para el negocio.

## Herramientas utilizadas

- Python
- pandas
- seaborn
- matplotlib
- Jupyter Notebook

## Principales hallazgos

- La mayor concentración de usuarios se encuentra en el segmento de **Uso medio**.
- Por edad, la categoría **Adulto** concentra la mayor cantidad de usuarios.
- Se identificaron valores extremos en la cantidad de mensajes, llamadas y minutos de llamada. Estos valores se conservaron al representar niveles de uso posibles y no existir evidencia de que fueran registros incorrectos.
- La frecuencia de usuarios dentro de un segmento no permite, por sí sola, determinar su rentabilidad o valor comercial. Para ello sería necesario incorporar variables económicas como ingresos, costos y rentabilidad.

## Ejecución del proyecto

El análisis completo se encuentra en:

`connectatel_usage_analysis.ipynb`

Para reproducir el análisis:

1. Descargar o clonar este repositorio.
2. Abrir el notebook en Jupyter Notebook, JupyterLab o Google Colab.
3. Tener disponibles los tres datasets utilizados en el proyecto.
4. Ajustar las rutas de los archivos CSV si es necesario.
5. Ejecutar las celdas del notebook en orden.

## Autor

Julio César Rodríguez Velásquez

Proyecto desarrollado como parte de mi formación en análisis de datos.
