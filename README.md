# Inventario Museo

Aplicación Java para la gestión de un inventario de museo.  
Incluye clases para manejar **categorías, objetos y ubicaciones**, además de pruebas unitarias con **JUnit 5**.

## Requisitos
- Java 17 o superior  
- (Opcional) Entorno de desarrollo como VS Code o IntelliJ IDEA

## Ejecución
PUEDES EJECUTAR EL .EXE DIRECTAMENTE
Compilado y empaquetado en `final.jar`.  
Para ejecutar la aplicación:

```bash
java -jar final.jar
```

La clase principal definida en el `MANIFEST.MF` es:

```
main.java.InventarioMuseo
```

## Estructura del proyecto
- `main/java/...` → Código fuente compilado
  - `InventarioMuseo` (clase principal)
  - `Categoria`
  - `Datos`
  - `Objeto`
  - `Ubicacion`
- `test/java/...` → Pruebas unitarias (`DatosTest`)
- `META-INF/` → Metadatos y licencias

## Dependencias
Incluye:
- [JUnit 5 (Jupiter API)](https://junit.org/junit5/) para pruebas unitarias
- API Guardian (`org.apiguardian.api`)

## Licencia
Archivos de licencia están disponibles en `META-INF/`.



---

# English Version

# Museum Inventory

Java application for museum inventory management.
Includes classes to handle **categories, objects and locations**, plus unit tests with **JUnit 5**.

## Requirements
- Java 17 or higher
- (Optional) A development environment such as VS Code or IntelliJ IDEA

## Running
YOU CAN RUN THE .EXECUTABLE DIRECTLY
Compiled and packaged in `final.jar`.
To run the application:

```bash
java -jar final.jar
```

The main class defined in `MANIFEST.MF` is:

```
main.java.InventarioMuseo
```

## Project Structure
- `main/java/...` → Compiled source code
  - `InventarioMuseo` (main class)
  - `Categoria` (Category)
  - `Datos` (Data)
  - `Objeto` (Object)
  - `Ubicacion` (Location)
- `test/java/...` → Unit tests (`DatosTest`)
- `META-INF/` → Metadata and licenses

## Dependencies
Includes:
- [JUnit 5 (Jupiter API)](https://junit.org/junit5/) for unit tests
- Guardian API (`org.apiguardian.api`)

## License
License files are available in `META-INF/`.

