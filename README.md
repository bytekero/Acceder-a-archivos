# 📂 Prácticas de Acceso a Datos: Manejo de Ficheros en Java

Este repositorio contiene una colección de ejercicios prácticos enfocados en la gestión de entrada y salida (I/O) de datos en Java. Se exploran tanto las clases clásicas de `java.io` como las modernas de `java.nio`.

## 🛠️ Tecnologías Utilizadas
* **Java Development Kit (JDK)**
* **Librerías:** `java.io` (File, FileReader, BufferedReader, PrintWriter, etc.) y `java.nio` (Files, Path, Paths).

## 🗂️ Estructura del Proyecto

El código se divide en ejemplos de lectura, escritura y manipulación de ficheros binarios.

### 1. Lectura de Ficheros de Texto

* **`LectorTexto.java`**: Programa robusto que recibe el nombre del archivo por argumentos. Realiza una comprobación de existencia y muestra dos métodos de lectura: carácter a carácter (`FileReader`) y línea a línea (`BufferedReader`).
* **`FichTextoLeer.java`**: Ejemplo básico que lee su propio código fuente (`FichTextoLeer.java`). Demuestra la lectura carácter a carácter y el uso de un array de char como buffer.
* **`FichTextoLeerNIO.java` (Actividad II)**: Implementación moderna utilizando `java.nio`. Usa la clase `Files` y `readAllLines` para cargar todo el contenido de un archivo en una lista de Strings de forma eficiente.

### 2. Escritura de Ficheros de Texto

* **`FichTextoBufEscribir.java` (Actividad IV)**: Escribe 10 líneas de texto en `FichTexto.txt`. Utiliza `BufferedWriter` y activa el modo *append* (`true`) para añadir contenido al final sin sobrescribir.
* **`FichTextoBufEscribir2.java` (Actividad V)**: Alternativa de escritura utilizando `PrintWriter`, que facilita la impresión de líneas formateadas. Sobrescribe el archivo en cada ejecución.
* **`EscribirNIO.java` (Actividad VI)**: Escritura moderna con `java.nio`. Demuestra el uso de `StandardOpenOption` para crear archivos si no existen (`CREATE`) o añadir contenido al final (`APPEND`).

### 3. Ficheros Binarios

* **`CopiarFicherosBytes.java` (Actividad VII)**: Utilidad para copiar cualquier tipo de archivo (texto, imagen, etc.). Lee bytes desde `Ffuente.txt` usando `FileInputStream` y los escribe en `Fdestino.txt` usando `FileOutputStream`.

## 🚀 Cómo Ejecutar

Para compilar y ejecutar cualquiera de los archivos, usa la terminal:

```bash
javac NombreArchivo.java
java NombreArchivo
