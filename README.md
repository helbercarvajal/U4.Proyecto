# 20191.DL Fundamentos de Deep Learning
     
## Proyecto U4: Redes Recurrentes

Para el presente proyecto, solo debe ejecutar el _notebook_ gaitAnalysis.ipynb

A continuación se indican las tareas realizadas de acuerdo con lo pedido en el curso:

- Dataset: señales triaxiales de acelerómetro y de giroscopio, adquiridas durante marcha libre en 6 pacientes con enfermedad de Parkinson (4 hombres y 2 mujeres, 69.67 +/- 6.86 años de edad) y 6 sujetos de control (3 hombres y 3 mujeres, 59.5 +/- 10.09 años de edad). Estas señales se descargan de Dropbox al ejecutar el _notebook_.

- Tarea de aprendizaje y métrica de evaluación: clasificación bi-clase (sano/enfermo). Se evaluó mediante el cálculo de la exactitud. Se aplicó _bootstraping_ con 10 repeticiones y a partir de esto se graficaron matriz de confusión, matriz de confusión normalizada, la curva de exactitud por repetición, curva de exactitud en conjuntos de entrenamiento y test, curvas de coste tanto en entrenamiento como en test, y curvas ROC.

- Estrategia de resolución:  se evaluaron 4 arquitecturas de redes recurrentes, dos de ellas basadas en LSTM. Se evaluaron los modelos para ambos pies en conjunto y de forma individual.
- Flujo de trabajo experimental:

        1. Diseño de 4 arquitecturas
            1.1 RNN simple seguida de una capa densa de 100 unidades
            1.2 LSTM seguida de una capa densa de 100 unidades
            1.3 GRU seguida de una capa densa de 100 unidades
            1.4 Tres capas de LSTM en cascada (16-32-16 unidades, respectivamente)
        2. Aplicación de las arquitecturas sobre las señales de ambos pies, pie derecho solo y pie izquierdo solo
        3. Validación mediante _bootstraping_
        4. Evaluación de las redes usando matrices de confusión, curvas de exactitud, de coste y ROC


### Integrantes

* CARVAJAL CASTAÑO HELBER ANDRÉS
* CASTRILLÓN OSORIO LUIS REINEL
* ROLDÁN VASCO SEBASTIÁN
