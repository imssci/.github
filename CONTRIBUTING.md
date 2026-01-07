# Guía de Contribución 🚀

¡Bienvenido al proyecto! Para mantener la estabilidad y calidad del código, seguimos este flujo de trabajo obligatorio bajo supervisión directa.

## 1. Asignación de Tareas
- **Solo el administrador asigna los Issues.** - No comiences a trabajar en una tarea si no te ha sido asignada formalmente en GitHub.
- Si tienes interés en un Issue libre, solicita la asignación en los comentarios del mismo.

## 2. Flujo de Ramas
- **main**: Código estable en producción. Solo el administrador realiza fusiones aquí.
- **dev**: Rama de integración donde se envían los cambios para revisión.
- **feature/issue-XX**: Ramas temporales para cada tarea (XX = número del issue).

## 3. Pasos para trabajar
1. **Crear rama local**: Siempre desde la versión más reciente de `dev`: 
   `git checkout dev && git pull origin dev`
   `git checkout -b feature/issue-XX`
2. **Desarrollo**: Realiza tus cambios y commits vinculándolos al issue:
   `git commit -m "Descripción breve #XX"`
3. **Push**: Sube tu rama a GitHub:
   `git push origin feature/issue-XX`

## 4. Pull Requests (PR) y Merge
- Abre el PR desde tu rama hacia **dev**.
- Es obligatorio incluir `Cierra #XX` en la descripción.
- Espera comentarios del administrador para realizar ajustes
- En caso de que no queden ajustes pendientes, el administrador hará merge con dev y podrás trabajar en el siguiente issue

## 5. Estilo de Commits (Semántico)
Usamos el estándar de *Conventional Commits* para que el historial sea legible:
- `feat:` Una nueva característica o funcionalidad.
- `fix:` Solución a un error (bug).
- `docs:` Cambios solo en la documentación.
- `style:` Cambios que no afectan el significado del código (espacios, formato, comas).
- `refactor:` Un cambio en el código que ni corrige un error ni añade una funcionalidad (mejorar lógica, limpiar nombres).
- `perf:` Un cambio en el código que mejora el rendimiento.
- `test:` Añadir pruebas que faltaban o corregir pruebas existentes.
- `chore:` Cambios en el sistema de construcción o herramientas auxiliares (como librerías de npm).