# Tarea TAS8 - Sentencias
## 1. Listar productos que no muestran pais de origen
  - Sentencia:
  ```
   SELECT (COUNT(*) - COUNT(country_of_origin)) AS "productos-sin pais"
FROM product;....
  ```
  - Captura:

<img src="./carpetas/CARPETAS /Captura de pantalla 2024-05-30 154947.png " alt="drawing" width="500"/>

## 2. Numero de clientes por ciudad..
  - Sentencia:
  ```
  
SELECT DISTINCT city, COUNT(city)
FROM clientes 
GROUP BY (city)....
  ```
  - Captura:

<img src="./carpetas/CARPETAS /Captura de pantalla 2024-05-30 154947.png  " alt="drawing" width="500"/>





