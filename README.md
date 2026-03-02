# 🎓 Sistema de Gestión de Información del Conocimiento Universitario
## Módulo: Innovación Curricular


---

## 📋 Descripción del Proyecto

Sistema de información web multicapa diseñado para gestionar el conocimiento generado en una universidad con sedes y seccionales en varias ciudades del país. Este proyecto permite registrar, consultar y analizar información académica, de investigación y curricular para apoyar la toma de decisiones y el mejoramiento continuo.

**Proyecto de Aula - Grupo 8**  
**Profesor:** Carlos Arturo Castro Castro

---

## 🏗️ Arquitectura del Sistema

El sistema está compuesto por **6 módulos** en una única base de datos relacional:

1. ✅ **Gestión Profesoral** (16 tablas)
2. ✅ **Innovación Curricular** (22 tablas) ← **NUESTRO MÓDULO**
3. ✅ **Mapa de Conocimiento** (18 tablas)
4. ✅ **Investigación** (16 tablas)
5. ✅ **Caracterización** (3 tablas)
6. ✅ **Gestión de Usuarios** (3 tablas)


<img width="552" height="621" alt="image" src="https://github.com/user-attachments/assets/77278dd3-8e57-4ba3-a2ab-4b4e329d97ec" />

📦 FASE 1: Tablas Sin Claves Foráneas (Primera Entrega - 06/03/2026)
Estas tablas son independientes y no dependen de ninguna otra. Se pueden crear, leer, actualizar y eliminar sin restricciones.

<img width="641" height="650" alt="image" src="https://github.com/user-attachments/assets/0d7dd716-c933-4ce3-a2bd-76dd702ebccb" />

 📊 Tabla 1: universidad
SQL



 CREATE TABLE universidad (
  id INT NOT NULL PRIMARY KEY,
  nombre NVARCHAR(60) NOT NULL,
  tipo NVARCHAR(45) NOT NULL,
  ciudad NVARCHAR(45) NOT NULL
);




📊 Tabla 2: aliado 


SQL
CREATE TABLE aliado (
  nit BIGINT NOT NULL PRIMARY KEY,
  razon_social NVARCHAR(60) NOT NULL,
  nombre_contacto NVARCHAR(60) NOT NULL,
  correo NVARCHAR(70) NOT NULL,
  telefono NVARCHAR(45) NOT NULL,
  ciudad NVARCHAR(45) NOT NULL
);






📊 Tabla 3: enfoque
SQL
CREATE TABLE enfoque (
  id INT NOT NULL PRIMARY KEY,
  nombre NVARCHAR(45) NOT NULL,
  descripcion NVARCHAR(45) NOT NULL
);




📊 Tabla 4: aspecto_normativo
SQL
CREATE TABLE aspecto_normativo (
  id INT NOT NULL PRIMARY KEY,
  tipo NVARCHAR(45) NOT NULL,
  descripcion NVARCHAR(45) NOT NULL,
  fuente NVARCHAR(45) NOT NULL
);









📊 Tabla 5: practica_estrategia 
SQL 
CREATE TABLE practica_estrategia (
  id INT NOT NULL PRIMARY KEY,
  tipo NVARCHAR(45) NOT NULL,
  nombre NVARCHAR(45) NOT NULL,
  descripcion NVARCHAR(45) NOT NULL
);







📊 Tabla 6: car_innovacion
SQL 
CREATE TABLE car_innovacion (
  id INT NOT NULL PRIMARY KEY,
  nombre NVARCHAR(45) NOT NULL,
  descripcion NVARCHAR(MAX) NOT NULL,
  tipo NVARCHAR(45) NOT NULL
); 






📊 Tabla 7: area_conocimiento
SQL 
CREATE TABLE area_conocimiento (
  id INT NOT NULL PRIMARY KEY,
  gran_area NVARCHAR(60) NOT NULL,
  area NVARCHAR(60) NOT NULL,
  disciplina NVARCHAR(60) NOT NULL
); 



## 👥 División de Trabajo - Fase 1

<img width="958" height="206" alt="image" src="https://github.com/user-attachments/assets/7262c355-cfe3-4bdd-a228-123113120f13" />
|

