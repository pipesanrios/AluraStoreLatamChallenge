# Alura Store Latam - Análisis de Ventas y Recomendación Final

Este proyecto consiste en el análisis de datos de ventas de cuatro tiendas de la cadena **Alura Store**, con el objetivo de identificar cuál de ellas presenta un desempeño inferior y, por ello, es candidata para ser vendida. El análisis se realizó utilizando **Python**, apoyándose en las bibliotecas **Pandas** para el manejo de datos y **Matplotlib** (y **Folium** en el análisis geográfico) para la generación de visualizaciones.

## Contenido del Proyecto

El notebook se divide en varios bloques de análisis que incluyen:

1. **Análisis de Facturación**  
   Se calculó la facturación total de cada tienda a partir de la suma de los precios de venta, obteniéndose las siguientes cifras:
   - **Tienda 1:** \$1,150,880,400.0
   - **Tienda 2:** \$1,116,343,500.0
   - **Tienda 3:** \$1,098,019,600.0
   - **Tienda 4:** \$1,038,375,700.0

   Se generó un gráfico de barras que resalta la tienda con menor facturación (Tienda 4) en color naranja.

2. **Ventas por Categoría**  
   Se analizó la distribución de ventas por categoría de productos en cada tienda. Esto permitió identificar las categorías más populares (como *Muebles*, *Electrónicos*, *Juguetes* y *Electrodomésticos*) y comparar la oferta de productos entre las tiendas mediante gráficos de barras horizontales.

3. **Calificación Promedio de Clientes**  
   Se evaluó la satisfacción de los clientes mediante el cálculo de la calificación promedio para cada tienda, obteniendo valores cercanos entre 3.98 y 4.05. Se generó un gráfico de barras con "zoom" en el eje Y para resaltar las sutiles diferencias en las calificaciones.

4. **Productos Más y Menos Vendidos**  
   Mediante el uso de la función `value_counts()`, se identificaron los productos con mayor y menor frecuencia de venta en cada tienda. Se generaron gráficos de barras para visualizar de forma comparativa tanto los productos más vendidos como los menos vendidos.

5. **Costo de Envío Promedio**  
   Se calculó el costo de envío promedio de cada tienda a partir de la columna "Costo de envío". Los resultados mostraron ligeras diferencias entre las tiendas, siendo Tienda 4 la que registró el costo más bajo, aunque este factor no compensó su menor facturación.

6. **Análisis Geográfico (Extra)**  
   Se exploraron las coordenadas geográficas (latitud y longitud) de las ventas para identificar patrones en la distribución de las compras. Se generaron:
   - **Gráfico de dispersión:** Visualizando las ventas geolocalizadas y coloreadas en función del precio.
   - **Mapa de calor (hexbin):** Para identificar áreas con mayor concentración de ventas.
   - **Mapa interactivo con Folium:** Con marcadores que permiten visualizar individualmente las ventas y obtener información adicional (por ejemplo, el precio).

## Herramientas Utilizadas

- **Python:** Lenguaje de programación.
- **Pandas:** Manipulación y análisis de datos.
- **Matplotlib:** Creación de gráficos estáticos.
- **Folium:** Generación de mapas interactivos.
- **Google Colab:** Entorno para ejecutar y compartir el notebook.

## Conclusión y Recomendación

**Hallazgos Integrados:**

- **Ingresos:** La Tienda 4 presenta la menor facturación total, indicando un desempeño comercial inferior.
- **Satisfacción del Cliente:** Aunque las calificaciones son similares entre todas las tiendas, Tienda 1 y Tienda 4 tienen valores ligeramente inferiores.
- **Portafolio de Productos:** El análisis de categorías y productos vendidos no mostró diferencias significativas que puedan compensar la brecha en ingresos.
- **Costos de Envío:** A pesar de contar con un costo de envío más bajo, la Tienda 4 no logra equilibrar su menor rendimiento comercial.
- **Análisis Geográfico:** Los patrones geográficos identificados apoyan la conclusión de que la Tienda 4 tiene un desempeño inferior en comparación con las demás.

**Recomendación Final:**  
Se recomienda **vender la Tienda 4**, ya que es la candidata que muestra un rendimiento inferior en términos de ingresos y eficiencia comercial, a pesar de tener algunas ventajas en costos logísticos. La venta de esta tienda permitirá redirigir recursos hacia aquellas unidades con mayor rentabilidad y potencial de crecimiento.
