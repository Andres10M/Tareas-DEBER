# View SQL
Vista cliente-invoice.
Vemos las columnas que necesitamos desde sus tablas originales  y las unimos con JOIN, lo siguiente es ejecutar:

1.- Creación de invoice_view
```
CREATE VIEW invoice_view AS SELECT i.id, i.code, i.create_at, i.total, c.full_name FROM invoice i JOIN client c  ON c.id = i.client_id;
```
Esto creara una vista del JOIN anterior.
Quedaría: 
<img src="carpetas/view/Captura de pantalla 2024-06-20 033945.png">

2.- Vista detail-product
```
CREATE VIEW detail_view AS SELECT d.id, d.quantity, p.description ,d.price, d.quantity * d.price AS subtotal FROM product p JOIN detail d ON p.id = d.productid;
```
Esta vista quedaría:
<img src="carpetas/view/Captura de pantalla 2024-06-20 035538.png">
