# Inventario Museo

[Español](#español) · [English](#english)

---

## Español

### Índice

- [Descripción](#descripción)
- [Funcionalidades](#funcionalidades)
- [Requisitos](#requisitos)
- [Cómo ejecutar](#cómo-ejecutar)
- [Datos de ejemplo](#datos-de-ejemplo)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Documentación de diseño](#documentación-de-diseño)
- [Tecnologías](#tecnologías)
- [Licencia](#licencia)

### Descripción

Aplicación de escritorio en **Java** para gestionar el inventario de un museo. Permite organizar los fondos del museo en **categorías**, **objetos** y **ubicaciones**, y guarda la información en archivos de texto locales.

Se distribuye lista para usar: `final.jar` contiene la aplicación compilada con todas sus dependencias, y también hay un ejecutable de Windows generado con Launch4j.

### Funcionalidades

- **Gestión de categorías**: alta y consulta de categorías del inventario.
- **Gestión de objetos**: nombre, descripción, fecha de alta, categoría y ubicación.
- **Gestión de ubicaciones**: almacenes o salas donde se guardan los objetos.
- **Persistencia en texto plano**: los datos se leen y escriben en `categorias.txt`, `objetos.txt` y `ubicaciones.txt`.
- **Interfaz de escritorio** con menús.
- **Pruebas unitarias** con JUnit 5 (`DatosTest`).

### Requisitos

- **Java 17 o superior** (`java -version` para comprobarlo).
- Windows, macOS o Linux.
- Opcional: un IDE como IntelliJ IDEA o VS Code para revisar el proyecto.

### Cómo ejecutar

**Opción 1 — Ejecutable de Windows** (la más sencilla):

```text
Gestión-museo-windowx64.exe
```

**Opción 2 — JAR** (multiplataforma):

```bash
java -jar final.jar
```

La clase principal es `main.java.InventarioMuseo`.

### Datos de ejemplo

El repositorio incluye los archivos de datos que usa la aplicación:

| Archivo | Formato | Ejemplo |
|---|---|---|
| `categorias.txt` | `id\|nombre` | `0\|Libros` |
| `objetos.txt` | `id\|nombre\|descripción\|fecha\|categoría\|ubicación` | `0\|@n0n#mbre\|Descripción\|2022-01-01\|0\|0` |
| `ubicaciones.txt` | `id\|nombre` | `0\|Almacén` |

Los campos están separados por `|`. Los identificadores de categoría y ubicación de `objetos.txt` apuntan a los de sus respectivos archivos.

### Estructura del proyecto

```text
Software-de-gestion-de-museo/
├── final.jar                        # Aplicación compilada con dependencias
├── Gestión-museo-windowx64.exe      # Ejecutable de Windows (Launch4j)
├── file.xml                         # Configuración de Launch4j
├── pom.xml                          # Metadatos Maven y dependencias (JUnit 5)
├── categorias.txt                   # Datos: categorías
├── objetos.txt                      # Datos: objetos
├── ubicaciones.txt                  # Datos: ubicaciones
├── diagramadeclases.puml            # Diagrama de clases (PlantUML)
├── diagramadecomponentes.puml       # Diagrama de componentes
├── diagramadenavegación.puml        # Diagrama de navegación
├── Proyecto/
│   └── META-INF/                    # Avisos de licencia de dependencias
├── LICENSE
└── README.md
```

### Documentación de diseño

Los tres archivos `.puml` se pueden abrir con [PlantUML](https://plantuml.com/) o con la extensión *PlantUML* de VS Code para generar los diagramas:

- **Clases**: modelo de datos (`Categoria`, `Objeto`, `Ubicacion`, `Datos`, `InventarioMuseo`).
- **Componentes**: separación entre interfaz, lógica y persistencia.
- **Navegación**: recorrido entre las pantallas de la aplicación.

### Tecnologías

- **Java 17**
- **Maven** (gestión de dependencias y build)
- **JUnit 5** (pruebas)
- **Launch4j** (empaquetado como `.exe`)
- **PlantUML** (documentación de diseño)

### Licencia

Este proyecto se distribuye bajo la **licencia MIT**. Consulta [LICENSE](LICENSE). Los avisos de licencias de terceros están en `Proyecto/META-INF/`.

---

## English

### Table of contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [How to run](#how-to-run)
- [Sample data](#sample-data)
- [Project structure](#project-structure)
- [Design documentation](#design-documentation)
- [Tech stack](#tech-stack)
- [License](#license)

### Overview

A **Java** desktop application for managing a museum inventory. It organizes the collection into **categories**, **objects** and **locations**, and stores the data in local text files.

It ships ready to run: `final.jar` contains the compiled application with all its dependencies, and there is also a Windows executable built with Launch4j.

### Features

- **Category management**: create and browse inventory categories.
- **Object management**: name, description, entry date, category and location.
- **Location management**: warehouses or rooms where objects are stored.
- **Plain-text persistence**: data is read from and written to `categorias.txt`, `objetos.txt` and `ubicaciones.txt`.
- **Desktop UI** with menus.
- **Unit tests** with JUnit 5 (`DatosTest`).

### Requirements

- **Java 17 or later** (check with `java -version`).
- Windows, macOS or Linux.
- Optional: an IDE such as IntelliJ IDEA or VS Code to inspect the project.

### How to run

**Option 1 — Windows executable** (easiest):

```text
Gestión-museo-windowx64.exe
```

**Option 2 — JAR** (cross-platform):

```bash
java -jar final.jar
```

The main class is `main.java.InventarioMuseo`.

### Sample data

The repository includes the data files used by the app:

| File | Format | Example |
|---|---|---|
| `categorias.txt` | `id\|name` | `0\|Libros` |
| `objetos.txt` | `id\|name\|description\|date\|category\|location` | `0\|@n0n#mbre\|Descripción\|2022-01-01\|0\|0` |
| `ubicaciones.txt` | `id\|name` | `0\|Almacén` |

Fields are separated by `|`. The category and location IDs in `objetos.txt` reference their respective files.

### Project structure

```text
Software-de-gestion-de-museo/
├── final.jar                        # Compiled app with dependencies
├── Gestión-museo-windowx64.exe      # Windows executable (Launch4j)
├── file.xml                         # Launch4j configuration
├── pom.xml                          # Maven metadata and dependencies (JUnit 5)
├── categorias.txt                   # Data: categories
├── objetos.txt                      # Data: objects
├── ubicaciones.txt                  # Data: locations
├── diagramadeclases.puml            # Class diagram (PlantUML)
├── diagramadecomponentes.puml       # Component diagram
├── diagramadenavegación.puml        # Navigation diagram
├── Proyecto/
│   └── META-INF/                    # Third-party license notices
├── LICENSE
└── README.md
```

### Design documentation

The three `.puml` files can be opened with [PlantUML](https://plantuml.com/) or the *PlantUML* extension for VS Code to render the diagrams:

- **Classes**: data model (`Categoria`, `Objeto`, `Ubicacion`, `Datos`, `InventarioMuseo`).
- **Components**: separation between UI, logic and persistence.
- **Navigation**: flow between the application screens.

### Tech stack

- **Java 17**
- **Maven** (dependency management and build)
- **JUnit 5** (tests)
- **Launch4j** (packaging as `.exe`)
- **PlantUML** (design documentation)

### License

This project is released under the **MIT License**. See [LICENSE](LICENSE). Third-party license notices are in `Proyecto/META-INF/`.
