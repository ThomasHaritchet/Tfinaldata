# Tfinaldata

Análisis y Predicción del Valor de Mercado de Futbolistas
Este proyecto tiene como objetivo analizar un conjunto de datos de futbolistas y construir un modelo de predicción para estimar el valor de mercado de los jugadores utilizando características como su edad, salario, nacionalidad y posición. El modelo desarrollado en este proyecto es un Random Forest Regressor.

Descripción del Proyecto
El dataset contiene información sobre futbolistas, incluyendo:

Nombre: Nombre del jugador.
Edad: Edad del jugador.
Posición: Posición en la que juega el futbolista.
Valor de Mercado (Value): Valor estimado del futbolista en millones de euros.
Salario (Wage): Salario del jugador en miles de euros.
Nacionalidad: País de origen del futbolista.
El objetivo principal es predecir el valor de mercado del jugador en función de otras variables disponibles en el dataset.

Enfoque
Carga y exploración del dataset:

Cargamos los datos desde un archivo CSV.
Realizamos una inspección inicial de los datos, eliminando columnas irrelevantes como "Name" y "Club".
Tratamos los valores nulos y se realizó una codificación de las variables categóricas, como la nacionalidad y la posición, para que pudieran ser utilizadas en el modelo.
Selección de características:

Decidimos usar un conjunto de características que creemos que tienen mayor relevancia para predecir el valor del futbolista: Edad, Salario, Posición y Nacionalidad.
Preprocesamiento de los datos:

Estandarización de las características numéricas (como la edad y el salario) para mejorar el rendimiento del modelo, asegurándonos de que todas las variables estén en la misma escala.
Eliminación de columnas irrelevantes (como Name y Club).
Construcción del modelo de predicción:

Se eligió el modelo Random Forest Regressor, que es adecuado para problemas con múltiples variables y relaciones no lineales.
Entrenamos el modelo usando un 80/20 split entre los datos de entrenamiento y prueba.
Evaluación del modelo:

Se utilizaron las métricas MSE (Error Cuadrático Medio) y R² (Coeficiente de Determinación) para evaluar el rendimiento del modelo.
El modelo alcanzó un R² de 0.74, lo que significa que puede explicar aproximadamente el 74% de la variabilidad en el valor de mercado de los futbolistas.
Resultados
MSE (Error cuadrático medio): 142917373750000.0
R² (Coeficiente de determinación): 0.7360137449189632
El modelo ha logrado predecir el valor de mercado de los futbolistas con un R² de 0.74, lo que indica un buen ajuste del modelo y una capacidad razonable para predecir el valor de mercado de los jugadores.

Conclusiones
El modelo Random Forest Regressor ha demostrado ser eficaz para predecir el valor de mercado de los futbolistas, con un rendimiento relativamente bueno (R² de 0.74).
Las variables como la edad, el salario y la posición de los futbolistas parecen tener un impacto importante en la predicción del valor de mercado.
A pesar de la complejidad de las relaciones en los datos, Random Forest ha logrado capturar bastante bien las interacciones entre las características.
Cómo ejecutar el proyecto
Clona este repositorio en tu máquina local:

bash
Copiar código
git clone <enlace-al-repositorio>
Instala las dependencias necesarias:

Copiar código
pip install -r requirements.txt
Abre el archivo Proyecto_PartIII_Apellido.ipynb en Jupyter Notebook o Google Colab y ejecuta las celdas para cargar, procesar los datos y entrenar el modelo.

Archivos incluidos
Proyecto_PartIII_Apellido.ipynb: Notebook con el código completo para la carga, procesamiento y modelado de los datos.
football_mini.csv: Dataset con la información de los futbolistas.
Dependencias
pandas
numpy
matplotlib
seaborn
scikit-learn
