# FUNCIONES SEGREGACIÓN.
## INSTRUCCIONES:
### 1.- Obtener la edad promedio de los miembros:

- Sentencia: 
 ```
SELECT AVG(age) AS average_age FROM Members;

  ```
 - Captura: 

 <img src = "carpetas/sum/Captura.png" width = "500">

---

### 2.- Obtener la edad mínima de los miembros:
- Sentencia: 
```
SELECT MIN(age) AS minimum_age
FROM Members;

```
- Captura:

<img src = "carpetas/sum/Captura de pantalla 2.png" width = "500">

---
### 3.- Obtener el número total de registros asistidos:
- Sentencia: 
```
SELECT COUNT(*) AS total_registrations
FROM Registrations;
```
- Captura:

<img src = "carpetas/sum/Captura de pantalla 3.png" width = "500">

---

### 4.-Obtener el número total de asistentes a todas las conferencias:
- Sentencia: 
```

```
- Captura:

<img src = "carpetas/sum/Captura de pantalla 4.png" width = "500">

---

### 5.-Obtener el número total de eventos por cada ciudad:
- Sentencia: 
```
SELECT city, COUNT(*) AS total_events
FROM Events
GROUP BY city;

```
- Captura:

<img src = "carpetas/sum/Captura de pantalla 5.png" width = "500">

---

### 6.-Obtener el número de registros por cada miembro:
- Sentencia: 
```
SELECT member_id, COUNT(*) AS registrations_count
FROM Registrations
GROUP BY member_id;

```
- Captura:

<img src = "carpetas/sum/Captura de pantalla 6.png" width = "500">

---

### 7.-Obtener el número de registros por cada conferencia:
- Sentencia: 
```

```
- Captura:
  
<img src = "carpetas/sum/Captura de pantalla 7.png" width = "500">

---


