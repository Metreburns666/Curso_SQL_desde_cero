# SQL y Bases de Datos desde Cero — MoureDev

![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=databricks&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL_8.4_LTS-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual_Studio_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Estado](https://img.shields.io/badge/Estado-Finalizado-success?style=for-the-badge)

## Descripción

Repositorio personal de aprendizaje desarrollado durante el curso **SQL y Bases de Datos desde Cero de MoureDev**.

El proyecto reúne documentación técnica, ejemplos de código, ejercicios resueltos y diagramas de bases de datos relacionales, organizados progresivamente en diez clases.

A lo largo del curso se trabajaron los fundamentos del lenguaje SQL, desde la configuración inicial de MySQL y la ejecución de consultas básicas hasta la administración de bases de datos, el diseño de relaciones entre tablas y la implementación de conceptos avanzados.

El repositorio conserva el material desarrollado durante el proceso de aprendizaje y permite consultar de manera organizada los conocimientos adquiridos.

## Estado del curso

| Indicador | Resultado |
|---|---|
| Clases completadas | 10 de 10 |
| Clases publicadas | 10 de 10 |
| Scripts SQL | 63 |
| Diagramas de bases de datos | 2 |
| Progreso académico | 100% |
| Certificación | Obtenida |
| Fecha de finalización | 24/11/2026 |
| Estado | Finalizado |

## Objetivos de aprendizaje

- Comprender los fundamentos de las bases de datos relacionales.
- Configurar y administrar un entorno local con MySQL.
- Consultar, filtrar, ordenar y transformar información mediante SQL.
- Insertar, actualizar y eliminar registros.
- Crear y administrar bases de datos y tablas.
- Aplicar restricciones de integridad.
- Diseñar relaciones entre entidades.
- Consultar información distribuida en múltiples tablas.
- Implementar índices, vistas, triggers y procedimientos almacenados.
- Comprender el funcionamiento de las transacciones.
- Organizar y versionar proyectos mediante Git y GitHub.

## Tecnologías y herramientas

| Tecnología | Aplicación |
|---|---|
| SQL | Lenguaje de consulta y administración de bases de datos. |
| MySQL Community Server 8.4.13 LTS | Motor de bases de datos relacionales. |
| MySQL Workbench | Administración gráfica, consultas y modelado de bases de datos. |
| Visual Studio Code | Desarrollo y organización de scripts SQL. |
| PowerShell 7.7.0 | Administración del entorno y ejecución de comandos. |
| Git | Control de versiones. |
| GitHub | Almacenamiento y publicación del proyecto. |
| Notion | Documentación y seguimiento académico. |
| Windows 11 | Sistema operativo del entorno de desarrollo. |

## Contenido del curso

Cada clase dispone de una carpeta independiente que contiene la documentación, los ejemplos o los ejercicios correspondientes.

| Clase | Tema | Contenido principal |
|---|---|---|
| 01 | [Introducción a MySQL Workbench](./Level%20One%20-%20MySQL%20Workbench/) | Instalación, configuración, conexiones y administración gráfica. |
| 02 | [SELECT](./Level%20Two/) | Consultas básicas y creación de una base de datos de práctica. |
| 03 | [Modificadores](./Level%20Three%20-%20modificadores/) | Filtrado, ordenamiento, agrupación, operadores y funciones. |
| 04 | [Escritura de datos](./Level%20Four%20-%20Escritura%20de%20datos/) | INSERT, UPDATE y DELETE. |
| 05 | [Administración de bases de datos](./Level%20Five%20-%20Adm%20Base%20de%20datos/) | Creación y eliminación de bases de datos. |
| 06 | [Administración de tablas](./Level%20Six%20-%20Adm%20de%20tablas/) | Creación, modificación, eliminación y restricciones de tablas. |
| 07 | [Creación de tablas relacionadas](./Level%20Seven%20-%20Creacion%20de%20tablas%20relacionadas/) | Relaciones 1:1, 1:N y N:M. |
| 08 | [Almacenamiento de datos relacionados](./Level%20Eight%20-%20Almacenamiento%20de%20datos%20relacionadas/) | Inserción de información en estructuras relacionales. |
| 09 | [JOIN](./Level%20Nine%20-%20Join/) | INNER JOIN, LEFT JOIN, RIGHT JOIN y UNION. |
| 10 | [Conceptos avanzados](./Level%20Ten%20-%20Conceptos%20Avanzados/) | Índices, triggers, vistas, procedimientos almacenados y transacciones. |

## Conocimientos desarrollados

### Consultas y recuperación de información

- SELECT
- DISTINCT
- WHERE
- ORDER BY
- LIKE
- AND, OR y NOT
- LIMIT
- IS NULL e IS NOT NULL
- IN
- BETWEEN
- Alias mediante AS

### Funciones y transformación de datos

- MIN y MAX
- COUNT
- SUM
- AVG
- CONCAT
- GROUP BY
- HAVING
- CASE
- IFNULL

### Manipulación de datos — DML

- INSERT
- UPDATE
- DELETE

### Definición y administración de estructuras — DDL

- CREATE DATABASE
- DROP DATABASE
- CREATE TABLE
- ALTER TABLE
- DROP TABLE
- ADD COLUMN
- RENAME COLUMN
- MODIFY COLUMN
- DROP COLUMN

### Restricciones e integridad de datos

- PRIMARY KEY
- FOREIGN KEY
- NOT NULL
- UNIQUE
- CHECK
- DEFAULT
- AUTO_INCREMENT

### Modelado relacional

- Entidades y atributos.
- Claves primarias y foráneas.
- Relaciones uno a uno (1:1).
- Relaciones uno a muchos (1:N).
- Relaciones muchos a muchos (N:M).
- Tablas intermedias.
- Integridad referencial.

### Consultas entre tablas

- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- UNION

### Conceptos avanzados

- Índices.
- Triggers.
- Vistas.
- Procedimientos almacenados.
- Transacciones.

## Base de datos de práctica — cineDB

Como parte del aprendizaje se desarrolló una base de datos relacional orientada al dominio cinematográfico, denominada `cineDB`.

Este entorno permitió aplicar consultas SQL sobre información relacionada con películas, personas, géneros cinematográficos, estudios y países.

Entre las entidades de la estructura inicial se encuentran:

| Tabla | Finalidad |
|---|---|
| countries | Almacenamiento de países. |
| genres | Clasificación de géneros cinematográficos. |
| studios | Información de estudios cinematográficos. |
| people | Información de personas vinculadas al cine. |
| movies | Información de películas. |
| movie_actor | Relación entre películas y actores. |
| movie_genre | Relación entre películas y géneros. |

La utilización de tablas relacionadas permitió trabajar con claves primarias, claves foráneas, relaciones de diferentes cardinalidades y consultas que combinan información de múltiples entidades.

La base de datos y los ejercicios fueron evolucionando a medida que se incorporaron nuevos conocimientos durante el curso.

## Diagramas de bases de datos

Durante el desarrollo del proyecto se incorporaron diagramas para representar gráficamente las estructuras relacionales trabajadas.

### Modelado de tablas relacionadas — Clase 7

![Diagrama de tablas relacionadas](./Level%20Seven%20-%20Creacion%20de%20tablas%20relacionadas/updated_db_2.png)

### Diagrama final — Clase 10

![Diagrama final de la base de datos](./Level%20Ten%20-%20Conceptos%20Avanzados/final_db.png)

Estos diagramas permiten visualizar las entidades, sus atributos y las relaciones establecidas entre las tablas.

## Organización del repositorio

El proyecto se encuentra organizado de manera progresiva mediante carpetas independientes para cada nivel de aprendizaje.

- Level One — Documentación introductoria.
- Level Two — Consultas SELECT y base de datos de práctica.
- Level Three — Modificadores y funciones.
- Level Four — Escritura de datos.
- Level Five — Administración de bases de datos.
- Level Six — Administración de tablas.
- Level Seven — Creación de tablas relacionadas.
- Level Eight — Almacenamiento de datos relacionados.
- Level Nine — JOIN.
- Level Ten — Conceptos avanzados.

Los archivos SQL incluyen ejemplos de los conceptos estudiados y ejercicios desarrollados durante el curso.

## Cómo utilizar este repositorio

### 1. Requisitos

- MySQL Community Server.
- MySQL Workbench o un cliente SQL compatible.
- Git.
- Un editor de código, como Visual Studio Code.

### 2. Clonar el repositorio

```bash
git clone https://github.com/Metreburns666/Curso_SQL_desde_cero.git
```

### 3. Acceder al proyecto

```bash
cd Curso_SQL_desde_cero
```

### 4. Configurar el entorno

Consultar la documentación de la [Clase 1 — Introducción a MySQL Workbench](./Level%20One%20-%20MySQL%20Workbench/README.md) para obtener información sobre la instalación, configuración y administración del servidor MySQL.

### 5. Preparar la base de datos de práctica

El archivo inicial de creación de la base de datos cinematográfica se encuentra en:

[Level Two — ejercicios_create_db.sql](./Level%20Two/ejercicios_create_db.sql)

Este archivo proporciona una estructura inicial para trabajar con los ejercicios correspondientes.

### 6. Explorar las clases

Se recomienda recorrer las carpetas siguiendo el orden numérico del curso.

Antes de ejecutar cada script, revisar:

- La base de datos seleccionada.
- Las tablas necesarias.
- Las dependencias entre entidades.
- Las operaciones que realiza el archivo.
- Los datos requeridos por cada ejercicio.

**Advertencia:** los scripts fueron desarrollados con fines educativos y algunos contienen operaciones que modifican o eliminan datos y estructuras, como DELETE, UPDATE, DROP TABLE y DROP DATABASE.

Se recomienda ejecutarlos exclusivamente en bases de datos de práctica, evitando entornos de producción.

Los archivos representan diferentes etapas del aprendizaje y no constituyen un único sistema de migraciones diseñado para ejecutarse automáticamente de principio a fin.

## Metodología de aprendizaje

El curso se desarrolló mediante una combinación de:

- Estudio de conceptos teóricos.
- Implementación de ejemplos prácticos.
- Resolución de ejercicios.
- Creación de estructuras relacionales.
- Experimentación con consultas SQL.
- Documentación de los conocimientos adquiridos.
- Organización del código por niveles.
- Control de versiones mediante Git.
- Publicación progresiva del material en GitHub.

La documentación académica complementaria y el seguimiento del progreso se organizaron mediante Notion.

## Competencias adquiridas

Al finalizar el curso se desarrollaron conocimientos prácticos en:

- Diseño y administración básica de bases de datos relacionales.
- Recuperación y manipulación de información mediante SQL.
- Construcción de consultas con múltiples condiciones.
- Agrupación y agregación de datos.
- Definición de estructuras y restricciones de integridad.
- Modelado de relaciones entre entidades.
- Consultas sobre múltiples tablas.
- Implementación introductoria de objetos avanzados de MySQL.
- Comprensión de transacciones y consistencia de datos.
- Documentación técnica y control de versiones.

Estos conocimientos constituyen una base aplicable al desarrollo backend, el análisis de datos y otros proyectos que requieren almacenamiento, procesamiento y recuperación de información estructurada.

## Certificación

El curso fue finalizado y aprobado el **24 de noviembre de 2026**, obteniendo el certificado de finalización correspondiente.

- Formación: SQL y Bases de Datos desde Cero.
- Plataforma educativa: MoureDev.
- Estado académico: finalizado y aprobado.
- Certificación: obtenida.
- Clases completadas: 10 de 10.

El certificado original se conserva de manera privada.

## Créditos y referencias

Este repositorio constituye un proyecto personal de aprendizaje basado en el curso SQL y Bases de Datos desde Cero de MoureDev.

Se reconoce la autoría del contenido formativo original y se agradece la disponibilidad de los recursos educativos utilizados.

### Recursos

- [MoureDev](https://mouredev.com/)
- [GitHub de MoureDev](https://github.com/mouredev)
- [Documentación oficial de MySQL](https://dev.mysql.com/doc/)
- [MySQL Workbench](https://dev.mysql.com/doc/workbench/en/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Documentación de Git](https://git-scm.com/doc)

---

**Proyecto de formación finalizado — Noviembre de 2026.**