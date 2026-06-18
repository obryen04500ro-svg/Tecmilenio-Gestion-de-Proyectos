# Comparación de Modelos Preentrenados de Hugging Face para Análisis de Sentimiento en Redes Sociales

## Descripción

Este proyecto presenta un análisis comparativo de modelos preentrenados de Hugging Face aplicados a una tarea de Procesamiento de Lenguaje Natural (NLP): clasificación de sentimiento en publicaciones de redes sociales.

La implementación fue desarrollada en Google Colab utilizando GPU y el ecosistema Hugging Face (Models, Datasets y Pipelines). Se evaluaron tres modelos especializados en análisis de sentimiento sobre el dataset **TweetEval**, comparando su desempeño mediante métricas estándar de clasificación y eficiencia computacional.

### Modelos evaluados

- RoBERTa Twitter (`cardiffnlp/twitter-roberta-base-sentiment-latest`)
- BERTweet Sentiment (`finiteautomata/bertweet-base-sentiment-analysis`)
- XLM-RoBERTa Twitter (`cardiffnlp/twitter-xlm-roberta-base-sentiment`)

### Métricas analizadas

- Accuracy
- Precision
- Recall
- F1-score
- Latencia promedio
- Throughput (textos por segundo)
- Intervalos de confianza mediante Bootstrap

### Objetivos

- Analizar el ecosistema Hugging Face para tareas de NLP.
- Comparar modelos preentrenados bajo las mismas condiciones experimentales.
- Evaluar el equilibrio entre precisión y eficiencia.
- Identificar el modelo más adecuado para un escenario de análisis de sentimiento.
- Documentar resultados, decisiones técnicas y riesgos de implementación.

### Resultados principales

Los experimentos mostraron que **RoBERTa Twitter** obtuvo el mejor desempeño general con un **F1-score macro de 0.7407**, mientras que **BERTweet Sentiment** presentó la menor latencia y el mayor throughput. Por su parte, **XLM-RoBERTa Twitter** destacó por su capacidad multilingüe, aunque no logró superar a los modelos especializados en inglés para este caso de uso.

### Tecnologías utilizadas

- Python
- Google Colab
- Hugging Face Transformers
- Hugging Face Datasets
- PyTorch
- Scikit-Learn
- Pandas
- Matplotlib


