# vehicles_project_sprint_7
Análisis exploratorio de datos de base de datos de vehículos y creación de una aplicación web con cuadros de mando para el despliegue de diferentes gráficos.

# Análisis de anuncios de venta de coches

## Descripción

Esta aplicación web fue desarrollada con **Streamlit**, **Pandas** y **Plotly** para realizar una exploración visual básica del conjunto de datos `vehicles_us.csv`.

La aplicación permite seleccionar mediante casillas de verificación los gráficos que se desean visualizar y generarlos al hacer clic en el botón **"Construir diagramas"**.

Actualmente se pueden construir:

* Un **histograma** para analizar la distribución del kilometraje (`odometer`).
* Un **gráfico de dispersión** para analizar la relación entre kilometraje (`odometer`) y precio (`price`).

Los gráficos son interactivos gracias a Plotly.

## Tecnologías utilizadas

* Python
* Pandas
* Plotly
* Streamlit



Archivos

* `vehicles_app.py` contiene el código de la aplicación Streamlit.
* `vehicles_us.csv` contiene el conjunto de datos utilizado por la aplicación.
* `README.md` contiene la documentación del proyecto.

## Instalación

Se recomienda utilizar un entorno virtual de Python.

Para instalar las dependencias necesarias, ejecutar:

```bash
pip install pandas plotly streamlit
```

También se pueden instalar las dependencias mediante un archivo `requirements.txt`:

```text
pandas
plotly
streamlit
```


## Ejecución de la aplicación

Ubicarse mediante la terminal en la carpeta donde se encuentran `vehicles_app.py` y `vehicles_us.csv`.

Luego ejecutar:

```bash
streamlit run app.py
```

Streamlit iniciará la aplicación y proporcionará una dirección local para acceder a ella desde el navegador.

## Uso de la aplicación

Al abrir la aplicación se muestra el encabezado:

**Análisis de anuncios de venta de coches**

La aplicación presenta dos casillas de verificación:

* **Construir un histograma**
* **Construir un gráfico de dispersión**

El usuario puede seleccionar una o ambas opciones.

Después debe hacer clic en:

**Construir diagramas**

### Histograma

Al seleccionar **"Construir un histograma"**, la aplicación genera un histograma utilizando la variable `odometer`.

Este gráfico permite observar la distribución del kilometraje de los vehículos incluidos en el conjunto de datos.

### Gráfico de dispersión

Al seleccionar **"Construir un gráfico de dispersión"**, la aplicación genera un gráfico utilizando:

* `odometer` en el eje X.
* `price` en el eje Y.

Este gráfico permite explorar visualmente la relación entre el kilometraje y el precio de los vehículos.


## Resultado esperado

La aplicación permite seleccionar independientemente uno o ambos gráficos.

Por ejemplo:

1. Seleccionar **Construir un histograma**.
2. Seleccionar **Construir un gráfico de dispersión**.
3. Hacer clic en **Construir diagramas**.
4. La aplicación mostrará ambos gráficos de forma interactiva.

Los gráficos pueden explorarse directamente desde la interfaz de Plotly, permitiendo acercar, alejar y examinar los datos.

## Datos

El archivo `vehicles_us.csv` contiene información sobre anuncios de vehículos usados. Entre las variables utilizadas por esta aplicación se encuentran:

* `odometer`: kilometraje del vehículo.
* `price`: precio del vehículo.

El análisis realizado por esta aplicación tiene un propósito exploratorio y no modifica el conjunto de datos original.
