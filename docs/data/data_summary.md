# Informe de datos

Los datos provienen del CMMS **SAP** donde cada tipo de evento ocurrido en las diferentes estaciones de petróleo es registrado, almacenando datos puntales que pueden ser de interes para realizar muchos tipos de análisis.

En este archivo se pueden identificar diferentes columnas que continen información detallada de cada registro o actividad. Este dataset se denomina **`qFallas`** el cual tiene diferentes tipos de datos como:

*   **`datetime64[ns]`** para identificar las fechas de los eventos como el inicio o el fin de la avería.
*   **`int64`** para identificar registros de conteo como el número del aviso o el número que identifica el equipo.   
*   **`float64`** para identificar registros cuantificados como la duración de la parada del equipo, clasificacion, proceso de gestión o el tipo de falla.
*   **`object`** para identificar todos los registros de texto como secuencia de caracteres (string) y corresponden a la gran mayoría de los datos del dataset. Tenemos ejemplos importantes como la descripción, el texto explicativo, la estación, el sistema, ubicción crticidad, etc.

Adiconalmente se cuenta con los datasets de los diccionarios y bolsas de palabras:

*   **`BoW clasificación de avisos`** 
*   **`Diccionario DA`**
*   **`Diccionario TE`**

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

El objetivo de este proyecto es diseñar una solución basa en *Procesamento de Leguaje Natural* **(NPL)** donde el algoritmo ingrese a cada uno de los textos de los eventos registrados, busque algunas palabras clave y encuentre patrones para que finalemente realice una clasificación de la siguiente manera:

![image](https://user-images.githubusercontent.com/119147133/205521661-d669ce31-588e-4e89-965e-967baafa19ab.png)

El algoritmo debe ingresar y validar cada uno de los textos de cada aviso y clasificarlo de acuerdo a la imagen anterior:

*   En la columna **`Clasificación`** debe colocar 0, 1, 2 o 3 para avisos pendientes, no aplican, condiciones o fallas.
*   En la columna **`Proceso de Gestión`** debe colocar 0, 1, 2, 3, 4 o 5 para avisos pendientes, no aplican, mantenimientos por condición, avisos de inteligencia artificial, eliminación de defectos o eventos de seguridad de procesos respectivamente.
*   En la columna **`Tipo de Falla/SP`** debe colocar 0 o 1 para avisos que estén pendientes o avisos que no apliquen.

La clasificación debe realizar en el siguiente orden lógico para lograr obtener una clasificación correcta:

![image](https://user-images.githubusercontent.com/119147133/205521667-4dda5a68-7549-43b9-9ec7-816d6a44f700.png)

Adicionalmente intentaremos realizar una predicción para los avisos los cuales cuentan unicamente con la descrición básica y de esta manera realizar una predicción previa lo cual permitirá anticiparnos a los difernetes eventos que se puedan presentar.

## Variables individuales

## Clasificación de las variables

## Relación entre las variables explicativas y la variable objetivo


