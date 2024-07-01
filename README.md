<p align="center">
  <img src="Data/sLf8WFANROO-ARRQrY0LiQ.webp" style="width: 150px;">
  
</p>
<h1 align="center">Clasificación multietiqueta de Tweets en español</h1>




### Descripción

Este proyecto aborda la clasificación multietiqueta de textos provenientes de redes sociales, específicamente tweets. El objetivo es etiquetar un conjunto de tweets de acuerdo a 11 sentimientos: `anger`, `anticipation`, `disgust`, `fear`, `joy`, `love`, `optimism`, `pessimism`, `sadness`, `surprise`, `trust`.
​Disponemos de un conjunto de 3561 tweets etiquetas para entrenar y validar el modelo o modelos necesarios, en el archivo 'sem_eval_train_es.csv'.


### Uso

### 1. Preprocesamiento y Limpieza de Texto
Para ejecutar el preprocesamiento y limpieza de texto, sigue las instrucciones en el notebook tarea-pln.ipynb. En este notebook, se han probado diferentes técnicas de procesamiento y limpieza de texto, incluyendo:

- Eliminación de caracteres especiales, links, menciones, hashtags.
- Conversión a minúsculas.
- Tokenización y vectorización usando técnicas como TF-IDF y embeddings.

#### 2. Modelos y Fine Tuning
En el notebook tarea-pln.ipynb también se ha explorado el uso de modelos preentrenados y el fine-tuning de los mismos. Se han evaluado varios modelos y técnicas:

- Modelos preentrenados (e.g., BERT, xml-RoBERTa).
- Fine-tuning de los modelos preentrenados en el conjunto de datos específico.
- Búsqueda de hiperparámetros utilizando Grid Search y Random Search.

#### 3. Evaluación del Modelo
Después de probar y evaluar diferentes modelos y técnicas, se ha seleccionado el mejor modelo basado en su rendimiento. Este modelo se ha utilizado para realizar predicciones sobre el conjunto ciego. Los resultados de la evaluación se encuentran en el notebook tarea-pln.ipynb

#### 4. Predicción final
Para predecir sobre el conjunto ciego, se ha utilizado el notebook Prediction-pln.ipynb.
 Este notebook aplica el modelo final seleccionado a los datos de prueba y genera las predicciones correspondientes.

### Datos

Los datos utilizados en este proyecto están en el directorio data/ e incluyen:

- **sem_eval_train_es.csv**: Conjunto de datos de entrenamiento.
- **sem_eval_test_es.csv**: Conjunto de datos de prueba.


### Estructura del repositorio
 <pre>
multi-label-tweet-classification/
│
├── data/
│ ├── sem_eval_train_es.csv
│ └── sem_eval_test_es.csv
│
├── tarea-pln.ipynb # Entrenamiento y evaluación de modelos
├── prediction.ipynb # Predicción sobre 
├── .gitignore
├── README.md
└── requirements.txt
</pre>


### Contribución
Si deseas contribuir o preguntar cualquier duda sobre este proyecto, ¡Contacta por LinkedIn! Y siéntete libre de crear pull requests con tus contribuciones.

### Créditos
Este proyecto ha sido desarrollado por Vicent Muñoz Correcher .

### Contacto
Para cualquier consulta, puedes contactarme a través de mi perfil de GitHub
