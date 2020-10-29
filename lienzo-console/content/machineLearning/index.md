+++
date = "2016-11-05T21:05:33+05:30"
title = "revenue"
+++

# Crear un modelo predictivo Machine Learning en IBM Cloud 

## Prerequisitos

```
$ Cuenta activa en IBM Cloud
```

## Crear servicios en IBM Cloud

Estos servicios son gratuitos en su versión lite.

```
$ Cloud Object Storage - Unidad de almacenamiento
$ Watson Studio - Ambiente de desarrollo para machine learning
$ Machine learning - Creación y despliegue de modelos
```

## Crear proyecto

Abrir el servicio de Watson Studio desde IBM Cloud o Watson Studio.

* En la pagina principal de Watson Studio hacer click en nuevo proyecto
* Darle un nombre al proyecto
* Escoger el servicio Object Storage que creado con anterioridad
* Crear
* Ir a cofiguración
* Bajar a servicios asociados
* Añadir servicio Watson
* Añadir el servicio Machine Learning
* En la sección de existentes agregar el servicio de Machine Learning ya creado

Se redirigue a la sección de servicios asociados.

## Data Asset

Ir a la pestaña de ***Assets*** o ***Activos*** y arrastrar los archivos en la sección load, al cargar un archivo se crea un data asset.

Al hacer click en el nombre del data asset se puede ver el botón refine o refinar, en esta sección se pueden analizar, remover columnas que no aportán al modelo y en la sección operación se pueden realizar operaciones y calculos complejos en la sección data.

En la sección perfil se pueden ver los datos distribuidos en columnas.

En la sección visualizaciones se pueden previsualizar, crear y descargar gráficos a raíz de los datos, se puede activar el flujo de datos con el boton en forma de triángulo y se puedén crear, salvar y ver los trabajos.

Al crear el flujo de trabajo, se debe configurar el ambiente de ejecución y se debe ejecutar el trabajo.

## Experimento AutoAI

El experimento AutoAI es un asistente para el entrenamiento de machine learning.

* Añadir experimento AutoAI
* Seleccionar desde proyecto
* Seleccionar el dato a predecir
* Ejecutar el experimento

Una vez que se realiza el experimento, automáticamente se particiona la data, se eligen los algoritmos y se ejecutan las interacciones.

En la comparación de interacciones o pipeline podemos ver los detalles de cada interacción.

En la sección de interconexión se pueden observar las interacciones del experimento y en cada interacción se puede guardar como modelo o com notebook. 

## Crear espacio de despliegue

* Hacer click en el modelo
* Visión general
* Promocionar al espacio de despliegue
* crear un nuevo espacio de despliegue
* Ascender

En Watson Studio 

* Ir a los espacios de despligue 
* Dirigirse a activos  
* Hacer click en el nombre del modelo
* Crear despliegue
* Ir a valores de espacio
* Ir a configuración
* Asociar instancia
* Seleccionar servicio machine learning
* Guardar
* Crear despliegue
* elegir *en linea* o *por lotes*
* crear

En el despliegue podemos ver una sección con assets de código, un end point, también hay una sección de pruebas.

Para poder realizar los despliegues se necesita contar con las [APIKeys](apikeys/), se pueden configurar en la sección IAM en Watson Studio