# comparativa modelos ML
## Objetivo
Dado un dataset de canciones de Spotify, que cuenta con 2017 diferentes canciones y un conjunto de atributos formado por **acustica**, **energia**, **instrumental**, **tempo**, **duracion**, entre otros datos relevantes de las canciones.

Además, contamos con una columna **target** que indica con un valor booleano si la canción es popular o no lo es.


Por lo tanto vamos a realizar aprendizaje supervisado para predecir si una próxima canción será popular o no. Para ello entrenamos varios modelos con diferentes algoritmos para poder comparar sus resultados y performance.
Los algoritmos utilizados son: **KNN** (K Nearest Neighbors), **SVM** (Support Vector Machine), **Random Forest** y **Perceptrones**
## Tecnologias
Para los algoritmos de clasificación y los indicadores del modelo [scikit learn](https://scikit-learn.org/).


Para la manipulación de datos [pandas](https://pandas.pydata.org/) y [numpy](https://numpy.org/).


Para los gráficos y visualización [seaborn](https://seaborn.pydata.org/) y [matplotlib](https://matplotlib.org/).
## Tecnicas
Para poder llevar a cabo el entrenamiento se utilizaron varias técnicas como:

**train-test-validation** donde se dividió el data set en 3 conjuntos. Uno de entrenamiento con el 60% del dataset, otro de prueba con un 20% y el último de validación con el 20% restante.

**cross-fold validation** (validación cruzada) se usaron 5 folds para validar el dataset con varios modelos.

**grid-search** (búsqueda en cuadrícula) para la búsqueda de los mejores hiperparametros y entrenar el modelo la combinación más óptima.

**tuning model** (ajuste de modelo) para mejorar los resultados del modelo modificando los distintos hiperparametros. 

**confusion matrix** (matriz de contingencia) para evaluar el valor real vs la predicción que realizó en modelo para sus 2 clases (positiva y negativa).

**data cleaning** (limpieza del dataset) se eliminaron columnas que no eran relevantes como el nombre de la canción y del intérprete.

No solo se analiza el **score** del modelo si no también variamos métricas de rendimiento como 
**precisión**, **exactitud**, **sesgo**, **F1 score** **TPR** (true positive rate), **TNR** (true negative rate), **FPR** (false positive rate) y **FNR** (false negative rate).
## Resultados
Observando los resultados podemos identificar 2 grupos. Uno con KNN y SVM, donde la matriz de contingencia dio prácticamente idéntica, y los parámetros de calidad también son bastante similares.

Y por otro lado tenemos random forest y perceptrones, en los cuales se obtuvieron resultados satisfactorios con índices muy altos.

No necesariamente estos resultados son la verdad absoluta y quiere decir que el algoritmo con los resultados más bajos es peor, y viceversa. Entra mucho en juego el dataset y el entrenamiento realizado.

En cuanto a coste computacional o tiempo de ejecución random forest es el más demandante.
SVM es quien le sigue en esta categoría pero está más controlado ya que solo se exploran valores para los parámetros **C** y **gamma**, pero si incluimos el parámetro **kernel** crece en gran medida el tiempo de ejecución.

Y por ultimo tenemos a KNN y perceptrones muy cercanos entre si y con la ejecución más rápida.