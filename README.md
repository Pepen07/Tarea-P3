# Sistema de Gestión de Biblioteca

Este proyecto es un sistema de gestión de biblioteca desarrollado en Python. Permite gestionar libros, usuarios, y operaciones de préstamo y devolución de libros. Además, incluye funcionalidades de búsqueda y pruebas unitarias para asegurar la calidad del sistema.

## Funcionalidades

- **Gestión de Libros:**
  - Añadir nuevos libros
  - Buscar libros

- **Gestión de Usuarios:**
  - Registrar nuevos usuarios

- **Operaciones de Préstamo:**
  - Prestar libros a los usuarios
  - Devolver libros

- **Pruebas Unitarias:**
  - Verificar el correcto funcionamiento de las operaciones de préstamo y devolución

## Estructura del Proyecto

- **Clases Principales:**
  - `Libro`
  - `Usuario`
  - `Biblioteca`

- **Pruebas Unitarias:**
  - `test_biblioteca.py`

## Ramas del Proyecto

- **main:** Contiene la versión estable del proyecto.
- **dev:** Rama de desarrollo principal.
- **qa:** Rama para pruebas y aseguramiento de la calidad.
- **feature/nueva-funcionalidad:** Rama para desarrollar nuevas funcionalidades.
- **hotfix/error-critico:** Rama para corrección de errores críticos.

## Flujo de Trabajo y Pull Requests

### Pull Request #1: Implementación de la estructura básica del sistema de biblioteca

- **Descripción:** Implementa las clases fundamentales del sistema de biblioteca.
- **Rama origen:** `dev`
- **Rama destino:** `main`

### Pull Request #2: Funcionalidad de préstamo y devolución de libros

- **Descripción:** Añade la lógica para prestar y devolver libros.
- **Rama origen:** `dev`
- **Rama destino:** `main`
- **Depende de:** PR #1

### Pull Request #3: Adición de pruebas unitarias

- **Descripción:** Desarrolla pruebas unitarias para verificar el funcionamiento del sistema.
- **Rama origen:** `qa`
- **Rama destino:** `dev`
- **Depende de:** PR #2

### Pull Request #4: Implementación del sistema de búsqueda de libros

- **Descripción:** Añade funcionalidad para buscar libros en el sistema.
- **Rama origen:** `feature/nueva-funcionalidad`
- **Rama destino:** `dev`

### Pull Request #5: Corrección de error crítico en la función de préstamo

- **Descripción:** Mejora el manejo de errores en la función `prestar_libro`.
- **Rama origen:** `hotfix/error-critico`
- **Rama destino:** `main`, luego a `dev` y `qa`

## Orden de Fusión Sugerido

1. **PR #1:** `dev` -> `main`
2. **Actualizar `dev`:** `main` -> `dev`
3. **PR #2:** `dev` -> `main`
4. **Actualizar `dev`:** `main` -> `dev`
5. **PR #3:** `qa` -> `dev`
6. **PR #4:** `feature/nueva-funcionalidad` -> `dev`
7. **PR #5:** `hotfix/error-critico` -> `main`, luego a `dev` y `qa`

## Cómo Contribuir

1. Clona el repositorio:
   ```bash
   git clone <URL-del-repositorio>
   cd <nombre-del-repositorio>
