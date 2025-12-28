El proyecto fue desarrollado originalmente como trabajo académico en Google Colab.

---
git 
# 🎭 Emotion Music – Training & Research

Este repositorio documenta la **Fase 1 (Investigación)** del proyecto integral **“Ponele música a tus emociones”**, desarrollado como trabajo final grupal. Aquí se encuentra la lógica de entrenamiento, el análisis de datos y la validación del motor de IA que da vida a la aplicación.

> **Nota de MLOps:** Este entorno es experimental. La arquitectura para transformar este modelo en un microservicio productivo y escalable se encuentra en el repositorio [emotion-music-mlops](https://github.com/ClaudiaMetz/emotion-music-mlops).

## 🚀 El Desafío: Sistema de Recomendación Extremo a Extremo

El objetivo del equipo fue construir una experiencia interactiva completa que superara la simple clasificación:

1. **Frontend (React):** Interfaz donde el usuario carga una fotografía personal.
2. **Análisis (Deep Learning):** Identificación de estados emocionales mediante el procesamiento de la imagen.
3. **Recomendación:** Selección de una temática musical basada en una estructura de categorías pareadas. La base de datos integrada asocia cada una de las 7 emociones detectadas (ej. Happy, Sad, Angry) con un set específico de tracks y un mensaje interactivo ad-hoc., basado en el sentimiento detectado.

## 🛠️ Stack Técnico (Fase de Investigación)

- **Framework de ML:** TensorFlow / Keras.
- **Arquitectura:** DenseNet (Transfer Learning).
- **Pre-procesamiento:** OpenCV.
- **Entorno de Desarrollo:** Google Colab / Jupyter Notebooks.

## 📊 Resultados y Decisiones Técnicas

El modelo fue validado buscando un equilibrio entre precisión y generalización para un entorno real:

- **Accuracy obtenido:** **66%** en el set de validación.
- **Criterio de Ingeniería:** Tras múltiples iteraciones de ajuste de hiperparámetros, se determinó que este nivel de precisión ofrecía la mejor estabilidad. Se priorizó la robustez del modelo ante nuevas imágenes, evitando el sobreajuste (_overfitting_) para asegurar la funcionalidad del MVP (Producto Mínimo Viable).

## 🚧 Estado del Proyecto y Reproducibilidad

- ✅ **Éxito Académico:** Proyecto aprobado con calificación 10/10.
- ⚠️ **Persistencia:** Siguiendo principios de **reproducibilidad**, este repo contiene el código necesario para replicar el entrenamiento. El modelo no se persiste como artefacto aquí; su versionado y servicio se gestionan en la etapa de Ops.
- 🔄 **Próxima Etapa:** Migración a una arquitectura de servicio profesional con **Docker** y despliegue en **Vertex AI (GCP)**.

---

🚀 _Si quieres ver cómo se llevó este modelo de un notebook a un contenedor listo para la nube, visitá el repositorio de [MLOps](https://github.com/ClaudiaMetz/emotion-music-mlops)._

Este repositorio **no está orientado a producción**.
