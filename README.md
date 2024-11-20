# Examen Técnico - Proyecto SPIRIT

Este examen técnico tiene como objetivo evaluar conocimientos en PHP y MySQL mediante la creación de una base de datos y tablas relacionadas.

## Requisitos

1. Crear una base de datos llamada **`secundaria`**.
2. La base de datos debe contener las siguientes tablas:
   - **Alumnos**
   - **Materias**
   - **Colegiaturas**

## Especificaciones de las Tablas

### Tabla `alumnos`
Esta tabla almacena información sobre los estudiantes.

- **Estructura**:
  - `id` (INT, AUTO_INCREMENT, PRIMARY KEY)
  - `id_materia` (INT, NOT NULL)
  - `nombre_completo` (VARCHAR(255), NOT NULL)
  - `edad` (INT, NOT NULL)
  - `grado` (VARCHAR(50), NOT NULL)
  - `fecha_registro` (DATETIME, DEFAULT CURRENT_TIMESTAMP)

### Tabla `materias`
Esta tabla contiene el listado de materias.

- **Estructura**:
  - `id` (INT, AUTO_INCREMENT, PRIMARY KEY)
  - `materia` (VARCHAR(255), NOT NULL)
  - `fecha` (DATE, DEFAULT CURRENT_DATE)

### Tabla `colegiaturas`
Esta tabla gestiona los pagos de colegiaturas.

- **Estructura**:
  - `id` (INT, AUTO_INCREMENT, PRIMARY KEY)
  - `id_usuarios` (INT, NOT NULL)
  - `costo` (DECIMAL(10, 2), NOT NULL)
  - `colegiatura_pagada` (BOOLEAN, DEFAULT FALSE)
  - `monto` (DECIMAL(10, 2), NOT NULL)

## Notas
- Utilizar claves primarias y relaciones foráneas si aplica.
- Asegurarse de que los nombres de las columnas coincidan con las especificaciones.
- Seguir las mejores prácticas de diseño de bases de datos.

## Instrucciones Adicionales

1. Implementar las tablas con los campos requeridos.
2. Probar las consultas necesarias para validar la creación y las relaciones.
3. Opcionalmente, integrar la base de datos con un backend en PHP para realizar operaciones CRUD.

---

¡Buena suerte en tu examen técnico! 😊
