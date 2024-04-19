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

El conjunto de datos seleccionado "Car details v3" incluye información detallada sobre coches usados a la venta en la India. Aquí hay un breve resumen de las características clave y los patrones observados en los datos:

### Características Principales:

* name: Marca y modelo del coche.
* year: Año de fabricación.
* selling_price: Precio de venta en rupias.
* km_driven: Kilómetros recorridos por el vehículo.
* fuel: Tipo de combustible (Diesel, Petrol, CNG, LPG, Electric).
* seller_type: Tipo de vendedor (Individual, Dealer, Trustmark Dealer).
* transmission: Tipo de transmisión (Manual o Automática).
* owner: Tipo de propiedad anterior (Primero, Segundo, Tercero, etc.).
* mileage: Eficiencia de combustible en km/l.
* engine: Capacidad del motor en CC.
* max_power: Potencia máxima en bhp.
* torque: Torque del motor.
* seats: Número de asientos.

### Resumen de Datos:

* Tamaño: El conjunto de datos inicialmente contiene 8,128 registros.
* Rango Temporal: Los coches abarcan desde el año 1983 hasta 2020.
* Precios: Varían considerablemente, con algunos coches listados tan bajos como ₹30,000 y otros hasta ₹10,000,000, mostrando una amplia gama de coches desde opciones económicas hasta vehículos de lujo.
* Kilometraje: Los coches han recorrido desde 1 km hasta más de 2.3 millones de km, indicando una mezcla de vehículos casi nuevos y otros extremadamente usados.
* Combustibles: Mayoritariamente, los coches utilizan diesel o gasolina, con una pequeña fracción usando CNG, LPG o siendo eléctricos.

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

## Conclusiones

Este conjunto de datos proporciona una rica fuente de información para comprender el mercado de coches usados en la India, ideal para futuros análisis más profundos como la predicción de precios o la evaluación de la depreciación del vehículo basada en diferentes características como el año, el tipo de combustible y el kilometraje.
