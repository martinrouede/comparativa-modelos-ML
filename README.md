# comparativa modelos ML

## Objetivo

**KNN** (K Nearest Neighbors), **SVM** (Support Vector Machine), **Random Forest** y **Perceptrones**

## Tecnologias

Para los algoritmos de clasificacion y los indicadores del modelo [scikit learn](https://scikit-learn.org/).

Para la manipulacion de datos [pandas](https://pandas.pydata.org/) y [numpy](https://numpy.org/).

Para los graficos y visualizacion [seaborn](https://seaborn.pydata.org/) y [matplotlib](https://matplotlib.org/).

## Tecnicas

Para poder llevar a cabo el entrenamiento se utilizaron varias tecnicas como:

**train-test-validation** donde se dividio el data set en 3 conjuntos. Uno de entrenamiento con el 60% del dataset, otro de prueba con un 20% y el ultimo de validacion con el 20% restante.

**cross-fold validation** (validacion cruzada) se usaron 5 folds para validar el dataset con varios modelos.

**grid-search** (busqueda en cuadricula) para la busqueda de los mejores hiperparametros y entrenar el modelo la combinacion mas optima.

No solo se analiza el **score** del modelo si no tambien variamos métricas de rendimiento como **precisión**, **exactitud**, **sesgo**, **F1 score**
 **TPR** (true positive rate), **TNR** (true negative rate), **FPR** (false positive rate) y **FNR** (false negative rate).

**confusion matrix** (matriz de contingencia) para evaluar el valor real vs la predicion que realizo en modelo para sus 2 clases (positiva y negativa).

**data cleaning** (impieza del dataset) se eliminaron columnas que no eran relevantes como el nombre de la cancion y del interprete.

## Resultados
