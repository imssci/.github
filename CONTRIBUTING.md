# Guía de Contribución 🚀

¡Bienvenido al proyecto! Para mantener la estabilidad y calidad del código, seguimos este flujo de trabajo obligatorio bajo supervisión directa.

## 1. Asignación de Tareas

- **Solo el administrador asigna los Issues.** - No comiences a trabajar en una tarea si no te ha sido asignada formalmente en GitHub.
- Si tienes interés en un Issue libre, solicita la asignación en los comentarios del mismo.

## 2. Flujo de Ramas

- **main**: Código estable en producción. Solo el administrador realiza fusiones aquí.
- **develop**: Rama principal de desarrollo e integración.
- **develop_fm**: Rama de integración específica para ciertos módulos (usar solo si se indica).

## 3. Pasos para trabajar

1. **Fork**: Realiza un fork de este repositorio a tu cuenta personal.
2. **Clonar**: Clona tu fork localmente y configura el repositorio original como `upstream`.
3. **Desarrollo**: Realiza tus cambios en tu fork. Asegúrate de estar sincronizado con la rama `develop` o `develop_fm` del repositorio original.
4. **Commits**: Mantén el estilo semántico vinculando el issue:
   `git commit -m "feat: descripción breve #XX"`

## 4. Pull Requests (PR) y Merge

- Abre el PR desde tu fork hacia **develop** o **develop_fm** (según se haya asignado la tarea).
- Es obligatorio incluir `Cierra #XX` en la descripción.
- Espera comentarios del administrador para realizar ajustes.
- Una vez validado, el administrador hará merge y podrás sincronizar tu fork.

## 5. Estilo de Commits (Semántico)

Usamos el estándar de _Conventional Commits_ para que el historial sea legible:

- `feat:` Una nueva característica o funcionalidad.
- `fix:` Solución a un error (bug).
- `docs:` Cambios solo en la documentación.
- `style:` Cambios que no afectan el significado del código (espacios, formato, comas).
- `refactor:` Un cambio en el código que ni corrige un error ni añade una funcionalidad (mejorar lógica, limpiar nombres).
- `perf:` Un cambio en el código que mejora el rendimiento.
- `test:` Añadir pruebas que faltaban o corregir pruebas existentes.
- `chore:` Cambios en el sistema de construcción o herramientas auxiliares (como librerías de npm).
