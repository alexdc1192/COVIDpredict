# COVIDpredict

## Project Description:

This project involves programming a simple Machine Learning model using only the following:

- Numpy library
- Math library
- Any built-in functions and classes

External tools such as Scikit-learn and Pandas are not allowed.

The model to be implemented is a K-NN (K Nearest Neighbours), which involves labeling or predicting new data based on its distance to the known data.

The model will be used to classify a group of patients into:

- Healthy (label value 0)
- Sick (label value 1)

The provided image demonstrates an example of K-NN.

![image](https://github.com/alexdc1192/COVIDpredict/assets/118775369/60ffacd2-123d-4372-b4dc-155e45f17921)

## Data Description:

The dataset contains two files that are read and stored in variables with the provided code. Both variables are arrays described below:

- Symptoms: an array with 2000 rows and 2 columns. Each row represents a patient, and each column represents a characteristic of that patient, specifically the body temperature in degrees Celsius and the blood oxygen concentration as a percentage.
- Labels: a one-dimensional array with 2000 values. Each value represents one of the 2000 patients. A value of 0 indicates a healthy patient, while a value of 1 indicates a patient with COVID.
![image](https://github.com/alexdc1192/COVIDpredict/assets/118775369/b4373866-275b-4769-acc4-3c0000b81e5c)

## Functionalities:

The program must have the following functionalities:

1. Data Splitting: The data needs to be divided into training and test sets to evaluate the model's performance. An 80-20 split will be performed, with 80% of the samples used for training and the remaining 20% for testing.

2. Data Standardization: Since the similarity between data is measured by distances, it is necessary to standardize all variables to have a mean of 0 and a standard deviation of 1.

3. Modeling: This part involves programming the data modeling to classify patients. The distances (similarities) between the new patient (from the test set) and the known healthy or sick patients (from the training set) will be calculated. The prediction will be based on the label of the nearest patient.

4. Model Performance Calculation: After obtaining the model, its effectiveness in classifying patients needs to be evaluated. The percentage of correct predictions made by the model will be calculated.





# COVIDpredict

## Descripción del proyecto 

Este proyecto consiste en programar un modelo sencillo de Machine Learning, usando unicamente:

- Librería Numpy
- Librería Math
- Cualquier función y clase built in

No se pueden utilizar herramientas extra, como por ejemplo:
- Librería Scikit-learn
- Librería Pandas

En este caso, el modelo será un K-NN (K Nearest Neighbours), 
que consiste en etiquetar o predecir nuevos datos en función de la distancia 
del nuevo dato a los datos ya conocidos.

El modelo servirá para clasificar una serie de pacientes en:

- Sano (en cuyo caso el valor de la etiqueta será 0)
- Enfermo (en cuyo caso la etiqueta será 1)


En la siguiente imagen se muestra un ejemplo de K-NN.
![image](https://github.com/alexdc1192/COVIDpredict/assets/118775369/60ffacd2-123d-4372-b4dc-155e45f17921)

En la imagen de la izquierda vemos como tenemos unos datos cuyas etiquetas son
conocidas - clase A o clase B -, y que tenemos una nueva muestra para clasificar.
En la segunda imagen es donde calculamos la similitud entre nuestra nueva
muestra y el resto. Para ello, calculamos la distancia entre las muestras. Por último,
tomamos los K valores más cercanos a nuestra muestra - en este caso los 3 más
cercanos - y vemos cuál es la clase mayoritaria. Vemos que de las tres muestras
más cercanas, 2 pertenecen a la clase B y una pertenece a la clase A, con lo que lo
más probable es que nuestra nueva muestra también pertenezca a la clase B.
Nota: con etiqueta nos referimos a la clase a la que pertenece cada muestra - en
este caso ‘sano’ o ‘enfermo’ -, que normalmente se codifica con un valor numérico.


## Descripción de los datos:

El dataset consta de dos ficheros que ya se leen y almacenan en variables con el
código que se os proporciona. Ambas variables son de tipo array y se describen a
continuación:
- Síntomas: array con 2000 filas y 2 columnas. Cada fila representa un
paciente y cada columna una característica de ese paciente. En este caso,
las características son la temperatura corporal en grados Celsius y la
concentración de oxígeno en sangre en porcentaje.
- Etiquetas: array unidimensional con 2000 valores. Cada valor representa a
uno de los 2000 pacientes. En caso de valer 0, el paciente está sano,
mientras que si vale 1, el paciente sufre de COVID.


En la siguiente imagen se observan las características de cada paciente - en el eje
Y la concentración de oxígeno en sangre y en el eje X la temperatura corporal -, así
como si está sano o enfermo - azul indica que el paciente está sano y naranja que
está enfermo.
![image](https://github.com/alexdc1192/COVIDpredict/assets/118775369/b4373866-275b-4769-acc4-3c0000b81e5c)


## Funcionalidades

El programa debe tener las siguientes funcionalidades:

- Separación de los datos en entrenamiento y test: cuando hacemos un
modelo, necesitamos saber cómo de bueno es para poder comparar y saber
qué opción es mejor.
Para ello, dividimos el conjunto en dos: el conjunto de entrenamiento y el de
test. El conjunto de entrenamiento serán los datos etiquetados que el modelo
utilizará, mientras que el conjunto de test servirá para saber cómo de bueno
es nuestro modelo, comparando la predicción del modelo con la etiqueta real.
Aquí, haremos una separación del 80% de las muestras en el conjunto de
entrenamiento y el 20% restante en el de test.

- Estandarización de los datos: como la similitud entre datos la vamos a medir
con distancias, necesitamos que todas las variables sean parecidas. Para
ello, vamos a forzar a nuestras variables a tener media 0 y desviación
estándar 1.

- Modelado: en esta parte programaremos la parte de modelado de datos para
clasificar a nuestros pacientes. Para ello, deberemos calcular las distancias
(similitudes) entre nuestro nuevo paciente - del conjunto de test - y los
pacientes que ya sabemos si están sanos o no - del conjunto de
entrenamiento. Nuestra predicción será la etiqueta del paciente más cercano.

- Calcular el rendimiento del modelo: Tras obtener nuestro modelo, queremos
saber cómo de efectivo es a la hora de clasificar a nuestros pacientes. Para
ello, vamos a calcular el porcentaje de veces que nuestro modelo acierta la
etiqueta correcta.



