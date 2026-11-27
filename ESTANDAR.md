# Estándar de codificación - Equipo 5

Lenguaje(s) del proyecto formativo: PHP, HTML, CSS, JavaScript y SQL (MySQL)

## 1. Nombrado
(pendiente)

## 2. Formato
(pendiente)

## 3. Comentarios y documentación
(pendiente)

## 4. Estructura de carpetas
(pendiente)

## 5. Git: ramas, commits y pull requests

### Ramas: dónde trabajamos

`main` es la rama principal del equipo. Antes de empezar una tarea, actualiza `main` y crea una rama para tu trabajo.

Usa el formato `tipo/nombre`, en minúsculas y sin tildes. Por ejemplo, Samuel usa `docs/samuel` para documentación y `fix/samuel` para corregir un error. Usa un nombre que te identifique dentro del equipo.

Si ya tienes una rama activa del mismo tipo, agrega una palabra que identifique la tarea, como `fix/samuel-login`.

### Commits: cómo guardamos los cambios

Un commit guarda un cambio. Haz uno por tarea pequeña y escribe el mensaje como `tipo: descripción breve`. El tipo va en inglés y el mensaje en español. Empieza con un verbo como *agregar*, *corregir* o *actualizar*.

| Tipo | Cuándo usarlo |
| --- | --- |
| `feat` | Agregas una función nueva. |
| `fix` | Corriges un error. |
| `docs` | Editas la documentación. |
| `refactor` | Ordenas el código sin cambiar lo que hace. |
| `test` | Agregas o cambias pruebas. |
| `build` | Cambias dependencias o herramientas de compilación. |
| `chore` | Haces mantenimiento, como configurar EditorConfig. |

Ejemplos: `docs: actualizar el readme` y `fix(login): corregir el mensaje de error`. La parte entre paréntesis es opcional e indica en qué parte del proyecto trabajaste.

Procura que el mensaje tenga máximo 72 caracteres y evita el punto final. Si hace falta más detalle, ponlo debajo del título, separado por una línea en blanco. Si el cambio hace que algo existente deje de funcionar como antes, avísalo con `!` antes de los dos puntos o explica qué deja de funcionar en una línea que empiece con `BREAKING CHANGE:`.

### Pull requests: cómo enviamos los cambios a revisión

Un pull request (PR) es una solicitud para incorporar los cambios de tu rama a `main`.

1. Usa tu propia cuenta de GitHub y verifica tu nombre y correo en Git. Antes de subir tus cambios, revisa los archivos y deja fuera contraseñas, datos personales, archivos temporales y cualquier archivo que no sea necesario para el proyecto.
2. Sube tu rama con `git push`, sin usar `--force`. Confirma en GitHub que aparece tu commit y abre un PR de tu rama hacia `main`.
3. Cuenta qué cambiaste y qué revisaste o probaste. Si el PR resuelve un issue, escribe `Closes #N` en la descripción. Reemplaza `N` por el número del issue, pegado al `#`.
4. Pide a alguien del equipo que revise el PR y atiende sus comentarios. Une los cambios a `main` cuando tengas al menos una aprobación y hayan pasado las comprobaciones que tenga el repositorio.
