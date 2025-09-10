# Taller_DAO
# Taller - Tecnologías de Persistencia con MyBatis

**Universidad de La Sabana**  
**Curso:** Diseño y Arquitectura de Software  
**Tema:** Frameworks de Persistencia – Introducción a MyBatis  
**Integrantes:** Julian Andres Vasquez Pedraza - Samuel Sabogal Espinel Leon - Santiago Buendia Londoño

---

## 📌 Descripción
Este proyecto implementa el uso de **MyBatis** como framework de persistencia, sobre una base de datos SQLite.  
Se configuran **mappers**, **resultMaps** y operaciones básicas de CRUD para el modelo de alquiler de películas.

---

## 🗄️ Configuración de la Base de Datos
- **Host:** `local/taller`  
- **Base de datos:** `jdbc:sqlite:bd.sqlite3`  
- **Driver:** `org.sqlite.JDBC`

---

## ⚙️ Parte I – Configuración Inicial

### 🔹 Configuración de MyBatis
En el archivo `mybatis-config.xml` (ubicado en `src/main/resources`), se agregaron los **typeAliases**:

```xml
<typeAliases>
    <typeAlias type="edu.unisabana.dyas.samples.entities.Cliente" alias="Cliente"/>
    <typeAlias type="edu.unisabana.dyas.samples.entities.Item" alias="Item"/>
    <typeAlias type="edu.unisabana.dyas.samples.entities.ItemRentado" alias="ItemRentado"/>
    <typeAlias type="edu.unisabana.dyas.samples.entities.TipoItem" alias="TipoItem"/>
</typeAliases>
