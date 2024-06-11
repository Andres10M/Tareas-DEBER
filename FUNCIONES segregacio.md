# FUNCIONES SEGREGACIÓN.
## INSTRUCCIONES:
### 1.- Obtener la edad promedio de los miembros:

- Sentencia: 
 ```
SELECT AVG(age) AS average_age FROM Members;

  ```
 - Captura: 

 <img src = "../../src/gbd-img-week8/first.png" width = "500" alt = "firstCapture">

---

### 2.- Obtener la edad mínima de los miembros:
- Sentencia: 
```
SELECT MIN(age) AS minimum_age
FROM Members;

```
- Captura:

<img src = "../../src/gbd-img-week8/second.png" width = "500" alt = "secondCapture">

---
### 3.- Obtener el número total de registros asistidos:
- Sentencia: 
```
SELECT COUNT(*) AS total_registrations
FROM Registrations;
```
- Captura:

<img src = "../../src/gbd-img-week8/third.png" width = "500" alt = "thirdCapture">

---

### 4.-Obtener el número total de asistentes a todas las conferencias:
- Sentencia: 
```

```
- Captura:

<img src = "../../src/gbd-img-week8/fourth.png" width = "500" alt = "fourthCapture">

---

### 5.-Obtener el número total de eventos por cada ciudad:
- Sentencia: 
```
SELECT city, COUNT(*) AS total_events
FROM Events
GROUP BY city;

```
- Captura:

<img src = "../../src/gbd-img-week8/fifth.png" width = "500" alt = "fifthCapture">

---

### 6.-Obtener el número de registros por cada miembro:
- Sentencia: 
```
SELECT member_id, COUNT(*) AS registrations_count
FROM Registrations
GROUP BY member_id;

```
- Captura:

<img src = "../../src/gbd-img-week8/sixth.png" width = "500" alt = "sixthCapture">

---

### 7.-Obtener el número de registros por cada conferencia:
- Sentencia: 
```

```
- Captura:

<img src = "../../src/gbd-img-week8/seventh.png" width = "500" alt = "seventhCapture">

---


