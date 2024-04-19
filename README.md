# PROYECTO_EDA

## Introducción EDA

Proyecto básico de EDA realizado en Python para proporcionar una visión clara y fundamental del conjunto de datos obtenido del siguiente enlace.

https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho

El Análisis Exploratorio de Datos (EDA) consiste de manera general en los siguientes pasos:

1) Cargar los datos: Usar la librería Pandas para cargar los datos desde el archivo CSV.
2) Inspección inicial: Verificar las primeras filas del conjunto de datos para entender la estructura y los tipos de datos.
3) Resumen estadístico: Proporcionar un resumen estadístico de las variables numéricas.
4) Tratamiento de valores nulos: Identificar y tratar los valores nulos en caso de existir.
5) Visualización de datos: Crear visualizaciones para entender de mejor manera la distribución de algunas variables y sus relaciones.

## Introducción al conjunto de datos

A continuación se indica una breve descripción de cada columna que forma parte del conjunto de datos.

* name: Nombre del modelo del coche.
* year: Año de fabricación del coche.
* selling_price: Precio de venta del coche.
* km_driven: Kilómetros conducidos.
* fuel: Tipo de combustible (Diesel, Petrol, etc.).
* seller_type: Tipo de vendedor (Individual, Dealer).
* transmission: Tipo de transmisión (Manual, Automatic).
* owner: Tipo de propiedad (First Owner, Second Owner, etc.).
* mileage: Rendimiento del combustible.
* engine: Capacidad del motor.
* max_power: Potencia máxima del motor.
* torque: Torque del motor.
* seats: Número de asientos.

## Tratamiento de valores nulos

Hay valores nulos en varias columnas (mileage, engine, max_power, torque, y seats). Estos valores nulos representan una pequeña fracción del total, pero deben ser tratados antes de realizar análisis más profundos o modelos de predicción.

Para simplificar el presente proyecto, se eliminan las filas con valores nulos; sin embargo, dependiendo del contexto y de la importancia de los datos, podrían imputarse estos valores utilizando métodos como la media, mediana, o modos, o incluso modelos predictivos.

## Resumen Estadístico

* year: Los autos en el dataset varían desde 1983 hasta 2020.
* selling_price: El precio de venta oscila entre ₹29,999 y ₹10,000,000 con una media de ₹638,271.
* km_driven: Los kilómetros recorridos varían desde 1 km hasta aproximadamente 2.36 millones de km, lo que sugiere la posible presencia de valores atípicos.
* seats: La mayoría de los autos tienen 5 asientos, aunque hay autos desde 2 hasta 14 asientos.

## Visualizaciones obtenidas

* Distribución de Precio de Venta: La mayoría de los coches tienen un precio de venta menor a ₹1,000,000, con una distribución sesgada hacia los precios más bajos.
* Distribución de Kilómetros Recorridos: La distribución muestra un sesgo hacia menos kilómetros recorridos, lo que es esperable en vehículos usados.
* Distribución de Año del Auto: Los autos tienden a ser de modelos más recientes, concentrándose principalmente entre 2010 y 2020.
* Distribución de Tipo de Combustible: La mayoría de los vehículos en el conjunto de datos utilizan diesel o gasolina, con pocos vehículos eléctricos o de GLP/CNG.

## Explicación del Script

1) Carga de datos: Utiliza Pandas para cargar los datos desde un archivo CSV.
2) Inspección inicial y resumen estadístico: Muestra las primeras filas y un resumen estadístico para entender las variables y sus distribuciones.
3) Tratamiento de valores nulos: Elimina las filas con valores nulos para simplificar el análisis inicial.
4) Visualizaciones:
* Histograma para la distribución del precio de venta.
* Histograma para la distribución de los kilómetros recorridos.
* Gráfico de cajas para ver la distribución de los años de los autos.
* Gráfico de conteo para los tipos de combustible.
