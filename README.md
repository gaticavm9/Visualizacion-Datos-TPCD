# Visualizacion de Datos
Aplicación en Jupyter Notebook que muestre una historia del proceso de visualización de datos para mostrar características del conjunto de datos seleccionado, utilizando las herramientas que provee el lenguaje de programación Python a través de las bibliotecas vistas en clases (Numpy, Pandas y Matplotlib).



## Instalación y uso del Notebook
Es necesario tener instalado el software Jupyter Notebooks y las librerías que se utilizarán.

### Jupyter Notebook
Para utilizar el software Jupyter Notebook se tienen distintas opciones, a continuación se listan las mas comunes:
- **Terminal**

Instalación
```bash
pip install notebook
```
Ejecución
```bash
jupyter notebook
```

- **Herramienta Anaconda**

Esta herramienta nos permite ocupar de manera sencilla notebooks de Jupyter ya que cuenta con las librerías de python más populares ya instaladas.

[Web Anaconda](https://www.anaconda.com/products/distribution).


### Librerías necesarias
Para instalar las librerías necesarias debemos ejecutar los siguientes comandos a través de la terminal.
- Numpy:
```bash
pip install numpy
```

- Pandas:
```bash
pip install pandas
```

- MatPlotLib:
```bash
py -m pip install matplotlib
```


### Utilizar Notebook
- **Terminal**

Descomprimir el notebook y abrir una terminal cambiando el directorio de trabajo actual a la ubicación en donde se encuentra nuestro notebook "main.ipynb".
```bash
cd Visualizacion-Datos-TPCD
```

O clonar el repositorio a través del comando [git clone](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository).
```bash
git clone https://github.com/victorex/Visualizacion-Datos-TPCD.git

cd Visualizacion-Datos-TPCD
```
Luego debemos ejecutar la aplicación Jupyter Notebook
```bash
jupyter notebook
```
Se abrirá un pestaña en el navegador donde debemos navegar a la carpeta donde tenemos nuestro notebook (Visualizacion-Datos-TPCD) y abrir "main.ipynb".

- **Anaconda**

En anaconda de igual manera abrimos la pestaña de Jupyter Notebook en el navegador, navegamos a la carpeta con los archivos necesarios (Tarea2-TPCD) y abrimos el archivo "Main.ipynb".

- **Visual Studio Code**

El proceso es similar a utilizar la herramienta de Anaconda, navegamos a la carpeta con los archivos necesarios (Tarea2-TPCD) y abrimos el archivo "Main.ipynb".

## Versión Python necesaria

    Python 3.8



## Propiedad de los datos
**Proyecto:** Plataforma de diagnóstico e historización del confort térmico, consumo de energía y calidad de aire en hospitales públicos.

**Director Proyecto:** Dr. Hugo Garcés H.

**ID Proyecto:** 18IIP-BB-99513.

**Instituciones Ejecutoras:**
- Universidad Católica de la Santísima Concepción (Campus San Andrés, Concepción)
- Universidad Técnica Federico Santa María (Sede Concepción)

**Datos:** Nodo (MAC FD:BA:37) Pasillo 5to Piso - Sector Neonatología del Hospital Regional Guillermo Grant Benavente.

## Variables

Análisis de Confort Térmico y Calidad del aire, mediante la definicion de confort térmico de la norma ISO 7730 y la norma ASHRAE 55-2013. El confort térmico es calculado mediante el Método Fanger.
 
**Atributos:**
|Atributo|Descripción|Indicador de Resultado|
|--------|--------|--------|
|Medición de confort térmico|Medición con nodo sensor de las variables que definen el confort térmico en un recinto: PMV: predicted mean vote y PPD: percentage persons dissastified|Presencia de medición de PMV y PPD en plataforma e interfaz de operación|
|Medición de calidad del aire interior|Medición con nodo sensor de las variables que determinan la calidad del aire interior: CO2, CO, NO2, COV (compuestos orgánicos volátiles); junto a mediciones de concentración de polvo grueso PM10 y polvo fino PM2.5|Presencia de medición de CO, CO2, NO2, COV, PM10, PM2.5 en plataforma e interfaz de operación|
|Registro historizado de mediciones|Mediciones almacenadas en base de datos con información asociada a tiempo en que la medición se ejecutó y ubicación en el recinto|Mediciones de las variables con formato {fecha-hora, valor}, factibles de ser analizadas con herramientas de series de tiempo|

**Índices:**
|Dato|Info|Unidad de medida|
|--------|--------|--------|
|id|ID del dato en la BD|U.A.|
|timestamp|Fecha y hora del dato capturado|Time|
|pmv|Voto Medio Previsto, estima la sensación térmica|U.A.|
|ppd|Porcentaje de Personas Insatisfechas|%|
|co2|Dioxido de Carbono|ppm|
|pm25|Material Particulado Fino|μg/m³|
|pm10|Material Particulado Grueso|μg/m³|
|temp|Temperatura|°C|
|hr|Humedad Relativa|%|
|voc|Compuestos Orgánicos Volatiles|ppm|
|co|Monoxido de Carbono|ppm|
|no2|Dioxido de Nitrogeno|ppm|
|c2h5ch|Etanol C2H5OH|ppm|
|idnodo|ID del nodo, correspondiente a su dirección MAC del dispositivo|U.A.|

**Diccionario:**
|Unidad|Descripción|
|--------|--------|
|ppm|Particulas por Millón|
|%|Porcentaje|
|Time|Instante de tiempo|
|μg/m³|Microgramos por metro cúbico|
|°C|Grados Celsius|
|U.A.|Unidad Adimensional|
