# CreditCardFraudDetectionML
Deteccion de fraudes de tarjetas de credito usando Machile Learning usando distintos algoritmos y haciendo comparaciones de rendimiento con respecto a la clasificacion de transacciones.

## Descripcion

El presente proyecto realiza una comparacion de algunos algoritmos de Machine learning aplicados al conjunto de datos de clasficaicon de transacciones fraudulentas de tarjetas de credito.

Debido a la gran cantidad de tecnicas de machine learning y de procesamiento de grandes cantidades de conjunto de datos se hace complicado obtener resultados buenos de clasificacion.

Es por ello que se realizan comparaciones entre un conjunto de datos sin procesar y procesado con distitas tecnicas de machine learning. Ademas se implementa AutoEncoding para ver que tan eficiente es clasificando este tipo de dataset.

### El Dataset

El conjunto de datos utilizado se puede encontrar [aqui.](https://www.kaggle.com/mlg-ulb/creditcardfraud)

El conjunto de datos se llama ```creditcard.csv```

Este dataset tiene 31 variables, de las cuales 28 estan reducidas dimensionalmente *(V1-V28)*, con el fin de transformar datos para proteger las identidades de las personas que han realizado las transacciones con tarjetas de credito.

Este dataset ha nacido capturando datos de transacciones bancarias de uno o mas bancos Europeos. No especifican que bancos o la cantidad de bancos. Aunque, podemos hacer la deduccion que ha sido un solo banco del continente Europeo debido a la estructura del dataset.

### Metodologia de Procesamiento y normalizacion

## Metodologia de Procesado y normalizacion

*   **Escalar valores:** Se escalan valores que tengan dispariedad en los rangos, mejorando el modelo de clasificacion
*   **Submuestreo aleatorio:** Se hace este submuestreo debido a la cantidad dispar de datos de una clase con respecto a otra.
*   **Construccion de un nuevo dataset:** Debido al submuestreo aleatorio nace la necesidad de construir un nuevo dataset con los datos seleccionados. Este conjunto de datos sera el definitivo.
*   **Particion del conjunto de datos:** Para poder problar los modelos de machine learning se hace una particion del conjunto de datos, escogiendo al azar 75% de los datos para entrenamiento y 25% para las pruebas. Estos fueron los mejores valores que he probado y que mejor resultado de clasificacion dan.

> Proximamente se analizaran datos atipicos en las variables y se les aplicara una metodologia de manejo de estos, con el fin de mejorar aun mas el modelo de machine learning.

## Ejecucion

Para poder ejecutar el presente proyecto se necesitan de las siguientes herramientas.

* **Python:** Se necesita Python en su version 3 o superior
* **TensorFlow:** Puedes instalar la version para CPu o para GPU.
* **SkLearn:** Necesario apra jecutar los algoritmos de ML, ademas de realizar las reducciones de dimensionalidad
* **MatPlotLib:** Permite la graficacion de datos, utilizado para graficar la distribuciones y frecuencias de algunas variables del conjunto de datos.
* **SeaBorn:** Complemento de MatPlotLib. Usado para graficar visualmente la matriz de confusion.
* **Tabulate:** Libreria para poder imprimir tablas de manera ordenada y con un formato agradable.
* **Numpy:** Necesario para el manejo de matrices, asi como realizar operaciones con ellas.
* **Pandas:** Libreria para el manejo de conjunto de datos y realizar operaciones con ella.

El proyecto se puede ejecutar tanto en la consola utilizando el siguiente comando teniendo el archivo ```.py```:
```
python CreditCardFraud.py
```
El archivo ```.ipynb``` se ejecuta en un entorno notebook python como Google Colab o Jupyter.


##Dependencias

Para instalar las dependencias debe de ejecutar los siguientes comandos:

* Numpy:
```
pip install numpy
```

* Pandas:

```
pip install pandas
```

* SkLearn:
```
pip install -U scikit-learn
```

* MatPlotLib:
```
pip install matplotlib
```

* Tabulate:

```
pip install tabulate
```

* Seaborn:
```
pip install seaborn
```

* TensorFlow:
```
pip install tensorflow==1.15      # CPU
pip install tensorflow-gpu==1.15  # GPU
```

## Construido con 

* [Python](https://www.python.org/) - Lenguaje de programacion usado para este proyecto
* [Pandas](https://pandas.pydata.org/) - Libreria que permite cargar y utilizar datasets y hacer operaciones de manera mas eficiente.
* [Sklearn](https://scikit-learn.org/stable/) - Ejecucion de los algoritmos de Preceptron multicapa, KNN, SVM, Random Forest, Regresion Logistica y Clasificador Uno vs el resto.
* [TensorFlow - Keras](https://www.tensorflow.org/) - Utilizacion para armar el autoenceder
* [Numpy](https://numpy.org/) - Manejo de matrices y operaciones de multiplicacion, y concatenacion
* [MatPlotLib](https://matplotlib.org/) - Permite la graficacion de datos
* [Seaborn](https://seaborn.pydata.org/) - Permite la graficacion de datos tabulados de manera mas eficiente que matplotlib
* [Tabulate](https://pypi.org/project/tabulate/) - Permite imprimir tablas de manera ordenada visualmente.

## Contribuyendo 

Por favor lee el CONTRIBUTING.md para detalles de nuestro código de conducta, y el proceso para enviarnos pull requests.

## Autores 

* **Carlos Garnica** - *Trabajo Inicial* - [Garnica1999](https://github.com/garnica1999)

También puedes mirar la lista de todos los [contribuyentes](https://github.com/Garnica1999/CreditCardFraudDetectionML/contributors) quíenes han participado en este proyecto. 

## Licencia 

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE.md](https://github.com/Garnica1999/CreditCardFraudDetectionML/blob/master/LICENSE) para detalles
