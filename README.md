# Predicción de depresión con Machine Learning

Este repositorio contiene un ejercicio académico de machine learning aplicado a un caso clínico. El objetivo es practicar Python y sus librerías (pandas, numpy, matplotlib y scikit-learn) construyendo un modelo sencillo que estima la probabilidad de recaída en depresión a los 6 meses.

> **Importante:** los datos son simulados. Este proyecto no es un producto clínico, no diagnostica y no debe usarse para tomar decisiones sobre pacientes reales.

## Contenido

- `Prediccion_Depresion_con_Machine_Learning.ipynb`: cuaderno con la generación de datos, exploración, entrenamiento, evaluación y prueba con pacientes de ejemplo.
- `README.md`: este documento.

## Problemática social

La depresión es uno de los trastornos mentales más frecuentes y una de las principales causas de discapacidad en el mundo. Afecta la vida laboral, académica, familiar y social, y se asocia con un mayor riesgo de recaída, deterioro funcional y conducta suicida. A pesar de su impacto, muchas personas no reciben atención oportuna por barreras como el estigma, el costo, la falta de profesionales, las listas de espera y la dificultad para acceder a un seguimiento continuo. En consultas breves, el psicólogo o la psicóloga debe evaluar muchos aspectos en poco tiempo, lo que puede limitar la detección temprana de factores de riesgo y el seguimiento longitudinal.

## Cómo se evalúa hoy y cuáles son sus límites

La evaluación psicológica combina la entrevista clínica, la observación, el juicio profesional y los instrumentos psicométricos. Uno de los más utilizados es el PHQ-9 (Patient Health Questionnaire-9), un cuestionario breve de 9 ítems basado en criterios del DSM para el cribado de depresión. Es rápido, económico, está validado en múltiples idiomas y produce un puntaje fácil de seguir en el tiempo.

Sin embargo, el PHQ-9 tiene limitaciones: es un autoinforme, depende de la interpretación del paciente, puede verse afectado por factores culturales, sociales o somáticos, y un puntaje de corte no equivale a un diagnóstico. Tampoco reemplaza la entrevista clínica ni permite comprender por sí solo el contexto, la comorbilidad o la evolución del paciente. Además, en la práctica el seguimiento suele ser discontinuo y los datos quedan dispersos en formatos distintos (papel, CSV, Excel, PDF), lo que dificulta su análisis conjunto.

## Por qué se usó este tipo de prueba

Se eligió un instrumento inspirado en el PHQ-9 porque:

- Es breve y de bajo costo, lo que facilita su aplicación en atención primaria y en seguimiento.
- Tiene una estructura estandarizada y un puntaje numérico, adecuado para un primer ejercicio de clasificación.
- Es ampliamente conocido y utilizado en investigación, lo que permite explicar el caso clínico con un lenguaje familiar.
- Permite trabajar variables clínicas y de seguimiento (síntomas, adherencia, apoyo social, sueño) sin usar datos reales.

En este ejercicio no se usa el PHQ-9 completo ni una muestra clínica real: se generan datos simulados y una variable simplificada (`phq9_alta`) para practicar el flujo de machine learning. El modelo no debe interpretarse como una validación clínica.

## Hacia dónde puede crecer el proyecto

Este ejercicio es una base. Para mejorar su precisión y utilidad se podría:

- Incorporar más variables clínicas y de seguimiento, con datos reales anonimizados y validación externa.
- Evaluar calibración, sensibilidad, especificidad y equidad del modelo en distintos grupos.
- Analizar sesgos y asegurar privacidad, consentimiento y protección de datos.
- Integrar una interfaz sencilla (por ejemplo, Streamlit o una aplicación web) donde el psicólogo o la psicóloga pueda subir un archivo CSV, Excel o el formato exportado de la prueba que utilice.
- Automatizar la lectura y validación de esos archivos, mostrar el riesgo estimado con una explicación breve y permitir que el profesional revise, corrija y decida.
- Mantener siempre el modelo como apoyo a la evaluación clínica, nunca como sustituto.

## Cómo ejecutar el cuaderno

1. Abrir el archivo `.ipynb` en Google Colab o Jupyter Notebook.
2. Instalar las dependencias si hace falta: `pandas`, `numpy`, `matplotlib` y `scikit-learn`.
3. Ejecutar todas las celdas en orden.

## Aviso ético

Los datos son ficticios y el proyecto tiene fines educativos. El PHQ-9 es una herramienta de cribado, no un diagnóstico. Si en un contexto real aparece riesgo suicida o ideas de muerte, se debe activar el protocolo clínico correspondiente de inmediato. No se deben subir datos identificables de pacientes a repositorios públicos.
