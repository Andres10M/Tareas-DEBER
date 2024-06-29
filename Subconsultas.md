# Subconsultas 
## Desarrollar los siguientes ejercicios usando subconsultas.
### DB FACTURAS
1.- Número total de facturas realizadas por cada cliente:

 nombre_cliente | direccion | nro_facturas

```
SELECT c.full_name, c.address, (SELECT COUNT(i.cliente_id) FROM invoice i WHERE c.id = i.cliente_id) FROM cliente c;
```
<img src = "carpetas/Subconsultas/Captura 1.png" width = "500">

2.- Listar nombre y correo de los clientes junto a su compra mas cara realizada:

nombres |  correo   | total_mas_alto
```
SELECT full_name, email, (SELECT MAX(total) FROM invoice i WHERE c.id = i.cliente_id) FROM cliente c;
```
<img src = "carpetas/Subconsultas/Captura 2.png" width = "500">

3.- Listar las facturas donde sus totales sean mayores al promedio de las facturas:

fecha_factura | total 
```
SELECT i.created_at, i.total FROM invoice i WHERE (SELECT AVG(i.total) FROM invoice i ) < i.total;
```
<img src ="carpetas/Subconsultas/Captura 3.png" width = "500">
 
 ---
 
### DB EVENT

1.- Listar una lista de conferencias, incluyendo el número total de asistentes registrados en cada conferencia:

id  | título | expositor | hora | día | total de asistentes | total de registros | 

```
SELECT c.id, c.title, c.speaker, c.hour, c.day,c.total_attendees, ( SELECT COUNT(*) FROM register r WHERE r.conference_id = c.id ) AS total_registered FROM conference c;
```
<img src = "carpetas/Subconsultas/Captura  4.png" width = "500">

2.- Listar los detalles de los miembros que asistieron a al menos una conferencia que tuvo más de 100 asistentes.

 id | nombre | email | edad |  

```
SELECT m.id, m.fullname, m.email, m.age FROM member m WHERE m.id IN ( SELECT r.member_id FROM register r JOIN conference c ON r.conference_id = c.id WHERE c.total_attendees > 50);
```
<img src = "carpetas/Subconsultas/Captura 5.png" width = "500">
