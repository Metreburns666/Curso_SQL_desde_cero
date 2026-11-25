# Clase 1 — Introducción a MySQL Workbench

> Curso SQL y Bases de Datos desde Cero — MoureDev

## 1. Introducción

En esta primera clase se abordaron los fundamentos del entorno de trabajo con MySQL, la configuración de una conexión local y la administración básica de bases de datos mediante MySQL Workbench.

El objetivo principal fue establecer un entorno funcional que permitiera trabajar posteriormente con el lenguaje SQL y las bases de datos relacionales.

## 2. Objetivos de aprendizaje

- Comprender la diferencia entre MySQL Server y MySQL Workbench.
- Configurar un entorno local de bases de datos.
- Administrar el servicio MySQL desde PowerShell.
- Establecer una conexión con el servidor.
- Familiarizarse con la interfaz gráfica de Workbench.
- Crear bases de datos y tablas.
- Definir columnas y tipos de datos.
- Insertar y visualizar registros.

## 3. Tecnologías y entorno de desarrollo

| Tecnología | Versión o configuración |
|---|---|
| Sistema operativo | Windows 11 |
| MySQL Community Server | 8.4.13 LTS |
| MySQL Workbench | Cliente gráfico |
| PowerShell | 7.7.0 |
| Servicio MySQL | MySQL84 |
| Puerto TCP/IP | 3306 |
| Tipo de inicio | Manual |

## 4. MySQL Server y MySQL Workbench

### MySQL Community Server

Es un sistema de gestión de bases de datos relacionales que permite almacenar, organizar, consultar y administrar información mediante el lenguaje SQL.

El servidor es el componente encargado de procesar las consultas y gestionar los datos.

### MySQL Workbench

Es una herramienta gráfica que permite interactuar con MySQL Server y facilita tareas como:

- Administración de conexiones.
- Creación de bases de datos.
- Creación y modificación de tablas.
- Ejecución de consultas SQL.
- Visualización y edición de registros.
- Diseño de modelos de bases de datos.

Workbench actúa como cliente del servidor MySQL y no reemplaza al motor de bases de datos.

## 5. Instalación del entorno

Las siguientes instrucciones constituyen una guía complementaria para reproducir el entorno utilizado durante el curso.

### MySQL Community Server

1. Acceder al sitio oficial de descargas:

   https://dev.mysql.com/downloads/mysql/

2. Seleccionar la versión LTS compatible con Windows.
3. Descargar y ejecutar el instalador correspondiente.
4. Configurar el servidor como servicio de Windows.
5. Establecer el puerto TCP/IP 3306.
6. Configurar una contraseña segura para el usuario administrador.
7. Completar la instalación y verificar el funcionamiento del servicio.

### MySQL Workbench

1. Acceder al sitio oficial:

   https://dev.mysql.com/downloads/workbench/

2. Seleccionar una versión compatible con el sistema operativo.
3. Descargar y ejecutar el instalador.
4. Completar la instalación.
5. Iniciar MySQL Workbench.

## 6. Administración del servicio MySQL desde PowerShell

Durante el curso se configuró el servicio MySQL con inicio manual, permitiendo controlar su ejecución desde la terminal.

Para iniciar o detener el servicio, se utilizó PowerShell con permisos de administrador.

### Iniciar el servicio

```powershell
Start-Service -Name MySQL84
```

### Consultar el estado del servicio

```powershell
Get-Service -Name MySQL84 | Select-Object Name, Status, StartType
```

### Detener el servicio

```powershell
Stop-Service -Name MySQL84
```

### Configurar el inicio manual

Como referencia complementaria, el tipo de inicio puede configurarse mediante:

```powershell
Set-Service -Name MySQL84 -StartupType Manual
```

### Interpretación de los estados

| Estado | Significado |
|---|---|
| Running | El servicio está en ejecución. |
| Stopped | El servicio está detenido. |
| Manual | El servicio no está configurado para iniciarse automáticamente con Windows. |

El nombre del servicio puede variar según la versión y configuración de MySQL instalada.

## 7. Configuración de una conexión local

Una vez iniciado el servidor, se configuró una conexión desde MySQL Workbench.

### Parámetros de conexión

| Parámetro | Valor |
|---|---|
| Connection Method | Standard (TCP/IP) |
| Hostname | 127.0.0.1 |
| Port | 3306 |
| Username | root |
| Password | Contraseña definida durante la instalación |

### Procedimiento

1. Abrir MySQL Workbench.
2. Crear una nueva conexión desde MySQL Connections.
3. Asignar un nombre descriptivo a la conexión.
4. Introducir los parámetros correspondientes.
5. Seleccionar Test Connection.
6. Introducir la contraseña del usuario.
7. Verificar que la conexión sea exitosa.
8. Guardar y abrir la conexión.

Durante la práctica se identificó y corrigió un error de conexión ocasionado por la utilización de un puerto incorrecto.

El puerto configurado en Workbench debe coincidir con el puerto utilizado por MySQL Server.

El usuario root se utilizó exclusivamente en un entorno local de aprendizaje. En entornos de producción se recomienda utilizar cuentas con permisos específicos.

## 8. Introducción a la interfaz de MySQL Workbench

Se exploraron los principales componentes de la herramienta.

| Componente | Función |
|---|---|
| MySQL Connections | Administración de conexiones. |
| Schemas | Visualización de las bases de datos disponibles. |
| Tables | Visualización de las tablas de un esquema. |
| SQL Editor | Escritura y ejecución de consultas SQL. |
| Result Grid | Visualización de los resultados y edición de registros cuando la consulta lo permite. |
| Action Output | Información sobre las operaciones ejecutadas y sus resultados. |

## 9. Creación de una base de datos

Durante la práctica se creó una base de datos denominada `hello_mysql`.

El procedimiento mediante la interfaz gráfica consiste en:

1. Acceder al panel Schemas.
2. Seleccionar Create Schema.
3. Introducir el nombre de la base de datos.
4. Seleccionar Apply.
5. Revisar la sentencia SQL generada por Workbench.
6. Confirmar la operación.
7. Verificar que el nuevo esquema aparezca en el panel correspondiente.

En MySQL, los términos schema y database se utilizan como equivalentes.

## 10. Creación de tablas

Dentro del esquema `hello_mysql` se creó una tabla denominada `users`.

### Estructura trabajada

| Columna | Finalidad |
|---|---|
| user_id | Identificación del usuario. |
| name | Nombre. |
| surname | Apellido. |
| age | Edad. |
| init_date | Fecha de inicio. |
| email | Correo electrónico. |

### Procedimiento mediante Workbench

1. Expandir el esquema correspondiente.
2. Acceder a la sección Tables.
3. Seleccionar Create Table.
4. Introducir el nombre de la tabla.
5. Definir las columnas y sus tipos de datos.
6. Revisar la estructura.
7. Aplicar los cambios.
8. Verificar que la tabla haya sido creada correctamente.

### Tipos de datos

Como referencia complementaria, algunos tipos de datos habituales en MySQL son:

| Tipo | Descripción |
|---|---|
| INT | Números enteros. |
| VARCHAR | Cadenas de texto de longitud variable. |
| DATE | Fechas. |
| DATETIME | Fechas y horas. |
| DECIMAL | Números decimales de precisión fija. |

La definición de tipos de datos adecuados permite representar correctamente la información almacenada en cada columna.

## 11. Inserción y visualización de registros

Se practicó la carga de información mediante la interfaz gráfica de MySQL Workbench.

### Procedimiento

1. Localizar la tabla `users` dentro del esquema.
2. Seleccionar la opción Select Rows - Limit 1000.
3. Introducir los valores correspondientes en la cuadrícula de resultados.
4. Seleccionar Apply.
5. Revisar y confirmar las operaciones generadas.
6. Comprobar que los registros hayan sido almacenados correctamente.

Durante la clase se cargaron y visualizaron seis registros de práctica.

Los valores originales no se incluyen en esta documentación para preservar la privacidad de los datos.

## 12. Comprobación del entorno

Al finalizar la clase se verificaron satisfactoriamente las siguientes operaciones:

- Inicio y detención del servicio MySQL.
- Consulta del estado del servicio desde PowerShell.
- Conexión local mediante MySQL Workbench.
- Creación de una base de datos.
- Creación de una tabla.
- Definición de columnas.
- Inserción de registros.
- Visualización de información almacenada.

También se contó con las bases de datos de ejemplo `sakila` y `world` como recursos adicionales de aprendizaje.

## 13. Conocimientos adquiridos

- Fundamentos de los sistemas de gestión de bases de datos relacionales.
- Diferenciación entre servidor y cliente de bases de datos.
- Administración básica de servicios en Windows.
- Configuración de conexiones locales.
- Identificación y resolución de errores básicos de conexión.
- Manejo introductorio de MySQL Workbench.
- Creación y exploración de esquemas y tablas.
- Inserción y visualización de datos.

## 14. Continuación del curso

A partir de la Clase 2, el aprendizaje se centra en la escritura y ejecución de sentencias SQL.

Los ejercicios y ejemplos de código se organizan en carpetas independientes y se versionan mediante Git y GitHub.

Esta primera clase se documenta mediante una guía técnica debido a que las prácticas se realizaron principalmente desde la interfaz gráfica de MySQL Workbench.

**Siguiente clase:** [Clase 2 — SELECT](../Level%20Two/)

## 15. Estado de la clase

- Estado: completada.
- Fecha de finalización: 19 de noviembre de 2026.
- Modalidad: teoría y práctica.
- Herramienta principal: MySQL Workbench.

---

## Créditos

Documentación elaborada como parte del proyecto personal de aprendizaje del curso SQL y Bases de Datos desde Cero de MoureDev.

- [MoureDev](https://mouredev.com/)
- [Documentación oficial de MySQL](https://dev.mysql.com/doc/)
- [Documentación de MySQL Workbench](https://dev.mysql.com/doc/workbench/en/)