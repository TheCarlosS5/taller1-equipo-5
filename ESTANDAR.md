# Estándar de codificación - Equipo 5

Lenguaje(s) del proyecto formativo: PHP, HTML, CSS, JavaScript y SQL (MySQL)

## 1. Nombrado

- Usar inglés de forma consistente en los identificadores del código y la base de datos; reservar el español para los textos de la interfaz y la documentación. No mezclar idiomas en un mismo identificador.
- Elegir nombres descriptivos y evitar abreviaturas poco claras, espacios, tildes y `ñ`.
- En PHP y JavaScript, nombrar variables, funciones y métodos con `camelCase` (por ejemplo, `userName`, `calculateTotal`); nombrar clases con `PascalCase` (por ejemplo, `UserController`) y constantes con `UPPER_SNAKE_CASE` (por ejemplo, `MAX_LOGIN_ATTEMPTS`).
- Nombrar archivos, carpetas, clases CSS e identificadores HTML con minúsculas y `kebab-case` (por ejemplo, `user-profile`, `main.css`); conservar nombres de entrada convencionales como `index.html` e `index.php`.
- En SQL, usar minúsculas y `snake_case`: nombres de tablas en plural (por ejemplo, `users`), columnas con nombres descriptivos (por ejemplo, `created_at`), clave primaria `id` y claves foráneas con el formato `<tabla_singular>_id` (por ejemplo, `user_id`).

## 2. Formato

Para mantener el código organizado, legible y uniforme, se establecen las siguientes reglas de formato:

### 2.1. Indentación
- Se utilizarán **4 espacios** para cada nivel de indentación.
- No se deben mezclar espacios y tabulaciones.
- El código debe mantener una estructura ordenada dentro de funciones, condicionales y ciclos.

### 2.2. Uso de comillas
- Se utilizarán comillas simples (`' '`) para cadenas de texto en JavaScript.
- Se utilizarán comillas dobles (`" "`) cuando el lenguaje o el formato del archivo lo requiera.
- Se mantendrá el mismo criterio en todo el proyecto.

### 2.3. Largo máximo de línea
- Se recomienda no superar los **120 caracteres** por línea.
- Cuando una instrucción sea demasiado extensa, se dividirá en varias líneas para facilitar su lectura.

### 2.4. Uso de llaves
- Las llaves de apertura y cierre (`{ }`) deben utilizarse en bloques de código como funciones, condicionales y ciclos.
- La llave de apertura se colocará en la misma línea de la declaración.
- La llave de cierre se ubicará en una línea independiente, alineada con el inicio del bloque.

**Ejemplo:**

```javascript
function saludar() {
    if (true) {
        console.log('Hola mundo');
    }
}

## 3. Comentarios y documentación

### Cuándo comentar
- Comentar **el porqué** (reglas de negocio, validaciones de seguridad, restricciones de base de datos o decisiones no evidentes), nunca repetir lo que ya expresa el código.
- No dejar código comentado en desuso ni notas temporales (TODO sin responsable) en main.
- Usar // para notas puntuales en PHP y JavaScript, /* ... */ en CSS y -- en scripts SQL.

### Cómo documentar funciones y archivos
- En PHP y JavaScript usar bloques **PHPDoc / JSDoc** (/** ... */) antes de funciones públicas y al inicio de cada archivo o módulo clave, indicando propósito, parámetros (@param) y retorno (@return).
- En HTML y CSS usar comentarios cortos únicamente para delimitar secciones principales de la interfaz.

### Qué debe tener el README.md
- Nombre, descripción breve del proyecto e integrantes del equipo (con usuario de GitHub).
- Requisitos del entorno (versiones de PHP, Apache/Laragon, MySQL/MariaDB y extensiones necesarias).
- Pasos claros de instalación, carga del esquema SQL y configuración local sin subir credenciales.
- Enlace al estándar de codificación (ESTANDAR.md) y a la documentación técnica del proyecto.

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
