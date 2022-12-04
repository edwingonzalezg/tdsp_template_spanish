# Informe de datos

Los datos provienen del CMMS **SAP** donde cada tipo de evento ocurrido en las diferentes estaciones de petróleo es registrado, almacenando datos puntales que pueden ser de interes para realizar muchos tipos de análisis.

En este archivo se pueden identificar diferentes columnas que continen información detallada de cada registro o actividad. Este dataset se denomina **`qFallas`** el cual tiene diferentes tipos de datos como:

*   **`datetime64[ns]`** para identificar las fechas de los eventos como el inicio o el fin de la avería.
*   **`int64`** para identificar registros de conteo como el número del aviso o el número que identifica el equipo.   
*   **`float64`** para identificar registros cuantificados como la duración de la parada del equipo, clasificacion, proceso de gestión o el tipo de falla.
*   **`object`** para identificar todos los registros de texto como secuencia de caracteres (string) y corresponden a la gran mayoría de los datos del dataset. Tenemos ejemplos importantes como la descripción, el texto explicativo, la estación, el sistema, ubicción crticidad, etc.

![image](https://user-images.githubusercontent.com/119147133/205521437-1d19199e-7617-46c3-a9bc-937340e24c17.png)

Adiconalmente se cuenta con los datasets de los diccionarios y bolsas de palabras:

*   **`BoW clasificación de avisos`** 
*   **`Diccionario DA`**
*   *   **`Diccionario TE`**

## Resumen general de los datos

*   **`qFallas`** archivo con la data extraída de SAP que contiene todos los registros.

![image](https://user-images.githubusercontent.com/119147133/205520784-0739fce8-6364-4577-8043-983807ae45d4.png)

*   **`BoW clasificación de avisos`** archivo que contiene una bolsa de palabras específicas de ingeniería depetróleos.

![image](https://user-images.githubusercontent.com/119147133/205521213-7325a928-1822-418a-a9e1-e51daa9e3a44.png)

*   **`Diccionario DA`** archivo que contiene un diccionario para realizar la corrección de palabras en la columna *descrición del aviso*. 

![image](https://user-images.githubusercontent.com/119147133/205521238-c70da6b2-e070-4222-87ed-a40028f55f0e.png)

*   **`Diccionario TE`** archivo que contiene un diccionario para realizar la corrección de palabras en la columna *texto explicativo*. 

![image](https://user-images.githubusercontent.com/119147133/205521255-19c941eb-2695-4f2a-a900-402515521c88.png)

## Resumen de la calidad de los datos



## Variable objetivo

## Variables individuales

## Clasificación de las variables

## Relación entre las variables explicativas y la variable objetivo


