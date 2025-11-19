# Detector de Spam

Este proyecto es un detector de spam simple que utiliza un clasificador Naive Bayes para identificar mensajes de spam en textos. El modelo se entrena con un conjunto de datos de mensajes etiquetados como spam o no spam.

## Descripción

El programa carga datos desde un archivo CSV (`data/spam.csv`), entrena un modelo de machine learning usando scikit-learn, evalúa su precisión y permite hacer predicciones rápidas sobre nuevos textos.

## Requisitos

- Python 3.7 o superior
- Las dependencias están listadas en `requirements.txt`

## Instalación

1. Clona o descarga este repositorio.
2. Navega al directorio del proyecto:

   cd spam_detector

3. Instala las dependencias:

   pip install -r requirements.txt

## Cómo ejecutar

1. Asegúrate de tener los datos en `data/spam.csv`.
2. Ejecuta el script principal:

    python src/spam_detector.py

3. El programa mostrará la precisión del modelo y una predicción de ejemplo.

## Mejoras posibles

- **Preprocesamiento de texto**: Agregar limpieza de texto (remover puntuación, convertir a minúsculas, stemming o lemmatización) para mejorar la precisión.
- **Modelos más avanzados**: Probar otros clasificadores como SVM, Random Forest o modelos de deep learning (e.g., LSTM con embeddings).
- **Validación cruzada**: Usar k-fold cross-validation para una evaluación más robusta.
- **Interfaz gráfica**: Crear una interfaz web con Flask o Streamlit para hacer predicciones en tiempo real.
- **Guardado del modelo**: Usar joblib para guardar y cargar el modelo entrenado, evitando retrainear cada vez.
- **Métricas adicionales**: Incluir precisión, recall, F1-score además de accuracy.
- **Dataset más grande**: Usar datasets más amplios o combinar múltiples fuentes de datos.
- **Feature engineering**: Explorar n-grams, TF-IDF en lugar de CountVectorizer.
