# instacart_data_wrangling
En este proyecto nos enfocaremos en la manipulación de datos (data wrangling). El proceso de preparación de los datos para su uso posterior, como el análisis. Este proceso normalmente implica eliminar defectos en los datos, agregar datos y visualizarlos. Básicamente, es todo lo necesario para preparar los datos para otros usos potenciales

# Introducción

Instacart es una plataforma de entregas de comestibles donde la clientela puede registrar un pedido y hacer que se lo entreguen, similar a Uber Eats y Door Dash. El conjunto de datos proporcionado tiene modificaciones del original. Se redujo el tamaño del conjunto para que tus cálculos se hicieran más rápido e introdujeron valores ausentes y duplicados. 

# Diccionario de datos

Hay cinco tablas en el conjunto de datos, y se tendrán que usar todas para hacer el preprocesamiento de datos y el análisis exploratorio de datos. A continuación se muestra un diccionario de datos que enumera las columnas de cada tabla y describe los datos que contienen.

1. instacart_orders.csv: cada fila corresponde a un pedido en la aplicación Instacart.
 * 'order_id': número de ID que identifica de manera única cada pedido.
 * 'user_id': número de ID que identifica de manera única la cuenta de cada cliente.
 * 'order_number': el número de veces que este cliente ha hecho un pedido.
 * 'order_dow': día de la semana en que se hizo el pedido (0 si es domingo).
 * 'order_hour_of_day': hora del día en que se hizo el pedido.
 * 'days_since_prior_order': número de días transcurridos desde que este cliente hizo su pedido anterior.

2. products.csv: cada fila corresponde a un producto único que pueden comprar los clientes.
 * 'product_id': número ID que identifica de manera única cada producto.
 * 'product_name': nombre del producto.
 * 'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
 * 'department_id': número ID que identifica de manera única cada departamento de víveres.

3. order_products.csv: cada fila corresponde a un artículo pedido en un pedido.
 * 'order_id': número de ID que identifica de manera única cada pedido.
 * 'product_id': número ID que identifica de manera única cada producto.
 * 'add_to_cart_order': el orden secuencial en el que se añadió cada artículo en el carrito.
 * 'reordered': 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.

4. aisles.csv
 * 'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
 * 'aisle': nombre del pasillo.

5. departments.csv
 * 'department_id': número ID que identifica de manera única cada departamento de víveres.
 * 'department': nombre del departamento.