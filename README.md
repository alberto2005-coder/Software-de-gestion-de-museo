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
