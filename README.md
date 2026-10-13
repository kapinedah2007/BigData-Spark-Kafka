Descripción de la solución

La solución desarrollada permite simular y analizar compras en tiempo real utilizando Apache Kafka y Apache Spark Structured Streaming.

El funcionamiento es el siguiente:

Un productor Kafka genera registros de compras de manera continua.
Los registros son enviados al tópico compras_online.
Spark Streaming consume los datos desde Kafka.
Los datos se agrupan por producto.
Se calculan estadísticas en tiempo real:
Total de compras por producto.
Ventas acumuladas.
Promedio de venta.
Los resultados se visualizan continuamente en la consola.
