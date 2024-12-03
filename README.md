# Conexión a Azure SQL Server y PostgreSQL en Databricks
![sql-psql-databricks](https://github.com/user-attachments/assets/d014ea09-577b-4999-9734-9ecb37650a84)

Este repositorio contiene una práctica que muestra cómo conectarse desde Databricks a dos bases de datos alojadas en Azure: Azure SQL Server y PostgreSQL. En este proyecto, se realizan consultas SQL para obtener información de las bases de datos y trabajar con ella utilizando PySpark.

## Descripción de la práctica
### Estructura de Archivos

Cada caso sigue una estructura de carpetas estándar:

- **`images/`**: Contiene las imágenes utilizadas en los análisis y visualizaciones.
- **`dataset/`**: Archivos de datos originales (en formatos .csv, .tsv, .xlsx, etc.) que se utilizarán para los análisis.
- **`solutions/`**: Carpeta donde se almacenan los notebooks resueltos, así como los datasets limpios resultantes de los análisis.
- **`resources/`**: Contiene los JDBC necesarios para conectar con las bases de datos MySQL y PostgreSQL.
  
En la raíz de cada caso, encontrarás:
- **Notebook vacío** para que puedas intentar replicar la solución por ti mismo.
- **README específico** para el caso en cuestión, explicando el objetivo y los pasos a seguir.

### Paso 1: Conexión a Azure SQL Server desde Databricks

1. Se configura la conexión JDBC para conectarse a una base de datos de Azure SQL Server.
2. Se establecen las credenciales de conexión, incluyendo el nombre de usuario, contraseña y la URL del servidor.
3. Se ejecutan diversas consultas SQL sobre la base de datos utilizando PySpark.

### Paso 2: Realización de Consultas en Azure SQL Server

Con la conexión establecida, se pueden realizar diversas consultas SQL sobre la base de datos. Algunos ejemplos incluyen:

1. Consultar todas las tablas en la base de datos.
2. Filtrar productos con precios mayores a 50.
3. Contar productos por categoría.
4. Calcular el precio promedio de todos los productos.

### Paso 3: Conexión a PostgreSQL en Azure desde Databricks

Una vez establecida la conexión a Azure SQL Server, se realiza la misma operación con PostgreSQL en Azure. La conexión se configura de manera similar a la anterior, pero con el controlador JDBC adecuado para PostgreSQL.

Con la conexión configurada, se pueden ejecutar consultas sobre PostgreSQL de manera similar a SQL Server.

## Requerimientos

1. **Databricks Community Edition** o **Databricks en Azure**.
2. **PySpark** para ejecutar las consultas en Databricks.
3. **Acceso a bases de datos Azure SQL Server y PostgreSQL**.

## Consideraciones

- Es necesario tener acceso de administrador a las bases de datos de Azure para realizar algunas consultas.
- Las configuraciones del servidor de bases de datos y las credenciales deben ser proporcionadas correctamente para establecer una conexión exitosa.
