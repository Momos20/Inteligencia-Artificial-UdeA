<img src="https://www.udea.edu.co/wps/wcm/connect/udea/721b156e-f6bc-4dc8-8595-8b4731c9a8c7/facultad-ingenieria.png?MOD=AJPERES&CVID=nc5CqsS" width=40% height=40% >


# Proyecto  de Inteligencia Artificial

Este repositorios se hace con el objetivo de desarrollar las actividades propuestas en la asignatura
de Inteligencia Artificial de la Universidad de Antioquia


## Miembros del equipo

- Nataly Rodriguez Ateourtua, C.C 1001505918, Bioingeniería
- Juan Camilo Cataño Zuleta, C.C 1001738289, Bioingeniería
- Daniel Enrique López Yepes, C.C 1000407016, Bioingeniería


## Set de datos

El set de datos que vamos a utilizar es [COVID-19 dataset](https://www.kaggle.com/datasets/georgesaavedra/covid19-dataset).
Este set de datos contiene información anonimizada de distintas partes del mundo, como lo es
Israel y Brasil, con el fin de analizar cómo es el comportamiento de la COVID-19.

El set de datos tiene mucha información según resultados de pruebas que se les practicaron
a los pacientes, con el fin de ver si las infecciones pueden arrojar algún patrón en estos
valores o si simplemente se generan de forma aleatoria.

## Cómo visualizar el set de datos

Para visualizar los datos en un notebook en colab basta con seguir los siguientes pasos:

1. Subir el archivo de credenciales kaggle.json al Colab, para ello se hace uso de las siguientes líneas de código:
    
```
  from google.colab import files
  files.upload()
  ! mkdir ~/.kaggle
  ! cp kaggle.json ~/.kaggle/
  ! chmod 600 ~/.kaggle/kaggle.json
```

Se abrirá un pequeño recuadro en el Colab que permite buscar directamente el archivo desde nuestro ordenador.

2. Descargar el set de datos directamente desde Kaggle, para ello hacemos uso de las siguientes líneas de código:

```
  ! kaggle datasets download -d georgesaavedra/covid19-dataset
```

Los datos se descargarán en un archivo comprimido de formato .zip

3. Descomprimir el archivo .zip, para ello usamos las siguientes líneas de código: 

```
  ! unzip /content/covid19-dataset.zip
```

Esto nos dejará un archivo .csv en nuestro directorio.

4. Abrir el dataset. (Si no se han instalado las librerías basta con correr la línea `import pandas as pd` y la línea `import numpy as np`, estas líneas cargan la librería Pandas y Numpy). Para ello ejecutamos la siguiente línea de código:

```
 pd.read_csv('owid-covid-data.csv') 
```

Y con ello los datos ya estarán disponibles. Es posible guardar también los datos haciendo ` miVariable=pd.read_csv('owid-covid-data.csv') ` y con ello los datos quedan guardados en una variable para su posterior uso.

## Entregas

Desde este espacio se puede acceder a las distintas entregas:
- [Primera entrega](https://github.com/Momos20/Inteligencia-Artificial-UdeA/blob/b0cacf560523fb09c669d7e65cb6a15951642628/PROYECTO_ENTREGA1.pdf)
- [Segunda entrega](https://github.com/Momos20/Inteligencia-Artificial-UdeA/blob/28eb865fb9d661947cf7869fa68f76ed275c7d55/PROYECTO_ENTREGA2.pdf)
- [Entrega final](https://github.com/Momos20/Inteligencia-Artificial-UdeA/blob/f900d43a2bddfa5ca4791d03a59eca75ba70b9cb/Proyecto_Entrega_Final.pdf)

## Videos

En este espacio se citan los videos respectivos para cada entrega:
- [Video de segunda entrega](https://youtu.be/JZYvBkXeqlo)
- [Video de entrega final](https://youtu.be/09nPtlonFYM)

## Notebooks

- 00-Visualización_de_datos [Abrir en Colab](https://colab.research.google.com/drive/1J0AHXn_1rpKEV7BYqP97OF-AP7u-i_73?usp=sharing)
- 01-Exploracion_de_datos [Abrir en Colab](https://colab.research.google.com/drive/1t7Hx43ng7wRH7bfk3ubl4hvc_WJT7wwf?usp=sharing)
- 02-Preprocesado_para_clasificación [Abrir en Colab](https://colab.research.google.com/drive/1FaWe5NcIFUU7UDhrMZByjnRHizD2kpud?usp=sharing)
- 03-Primer_Modelo_Regresión_Lineal [Abrir en Colab](https://colab.research.google.com/drive/16dxO2VbSLnJAbqaqDkOcUt-aCfO9El-R?usp=sharing)
- 04-Segundo_Modelo_Árboles_de_Decisión [Abrir en Colab](https://colab.research.google.com/drive/1H8aU1viJCA9d8kyVJTurBvQZFiVHElZD?usp=sharing)
- 05-Tercer_Modelo_Perceptrón_Multicapa [Abrir en Colab](https://colab.research.google.com/drive/1axxiZSsISRDT7VXkEYwXxWqHmhQxlJwA?usp=sharing)
- 06-Cuarto_Modelo_Máquina_de_Soporte_Vectorial [Abrir en Colab](https://colab.research.google.com/drive/1j0jD-Y9N4FMEsZwtBw4ckqzNQhzjlS2j?usp=sharing)
- 07-Quinto_Modelo_Regresión_Logística [Abrir en Colab](https://colab.research.google.com/drive/1JSby_teJkdbeh8SBfH86LtdJeX77gfKS?usp=sharing)

## Agradecimientos

Agradecemos al profesor Raúl Ramos Pollán, quién fue nuestro docente y guía durante este semestre, gracias a él pudimos realizar todo lo que se encuentra aquí.
