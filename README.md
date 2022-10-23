# ML and DL Diagnosis of pneumonia given Xray images

Diagnóstico de neumonía dadas imágenes de Rayos X de pacientes con neumonías y normales

Hipótesis: clasificar correctamente a pacientes con neumonía dadas imágenes en Rayos X con diagnóstico normal y de neumonía.

Lo más importante es predecir correctamente a los pacientes con neumonía. Conlleva más riesgo clasificar sin neumonía a un paciente con neumonía que al contrario (error tipo I), por lo que quiero minimzar los Falsos Negativos.

Dado el desequilibrio de clases, elijo el estadístico Kappa para evitar obtener una alta precisión al adivinar siempre la clase más frecuente. El estadístico kappa solo recompensará al clasificador si es correcto con más frecuencia que esta estrategia simplista.

También quiero conseguir un buen estadístico de sensibilidad prediciendo la mayor cantidad de pacientes con neumonía de todos los pacientes con neumonía existentes. Y una buena precisión del valor positivo predictivo (acertar la mayor cantidad de pacientes con neumonía del total de pacientes con neumonía predichos).

Técnicas a utilizar, diferentes técnicas de ML para clasificación y DL con uso de keras:
* K-Means: método sencillo y rápido para empezar a explorar.
* Naive Bayes: método eficinte y no sesgado por valores atípicos.
* Bagging: método que intenta reducir el error aprovechándose de la indepdencia que hay entre los algoritmos simples.
* Random Forest: método que permite manejar grandes cantidades de datos con mayor dimensionalidad (transformaré las imágenes para que sean 100x100, por tanto, 100001 dimensiones)
* Support Vector Machine: método no sensible al sobreajuste y suele tener alto rendimiento.
* Regresión Logística: tiene enfoque probabilístico.
* keras: librería para trabajar con imágenes y hacer uso del Deep Learning.


