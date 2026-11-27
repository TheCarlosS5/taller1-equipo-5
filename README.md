# Equipo 5 - los hijos de Elon Musk

## Descripción

Taller 1 del Equipo 5 sobre Git y GitHub. El proyecto incluye una página HTML de ejemplo y las fichas de presentación del equipo. El taller sirve para practicar el trabajo colaborativo con ramas, issues, pull requests y resolución de conflictos.

Consulta nuestro [estándar de codificación](ESTANDAR.md).

## Integrantes

- Carlos Stiven Gutiérrez Ramírez — [@TheCarlosS5](https://github.com/TheCarlosS5)
- Camilo Andrés Tamayo Durán — [@copito111](https://github.com/copito111)
- Kevin Fernando Martínez Pérez — [@Fernando1658](https://github.com/Fernando1658)
- Samuel Santiago Ramírez Fierro — [@Santiagopro23YT](https://github.com/Santiagopro23YT)
- Santiago Ortiz Claros — [@Ortiz-png](https://github.com/Ortiz-png)

## Cómo clonar el repositorio

Abre una terminal y ejecuta estos comandos:

```bash
git clone https://github.com/TheCarlosS5/taller1-equipo-5.git
cd taller1-equipo-5
```

## Instrucciones del taller

1. Un integrante crea el repo y agrega a los demás como colaboradores.
2. Crean un issue por tarea: cada uno agrega su sección a index.html.
3. Cada integrante actualiza `main` y crea una rama con el formato `tipo/nombre`, por ejemplo `feat/samuel`.
4. Guarda tus cambios con un commit y sube tu rama. Abre un PR hacia `main` y explica qué cambiaste y qué verificaste. Si el PR resuelve un issue, añade `Closes #N` en la descripción y reemplaza `N` por su número.
5. Pide a otro integrante que revise el PR. Integra los cambios después de recibir al menos una aprobación y pasar las comprobaciones del repositorio.
6. Dos integrantes editan la misma línea y resuelven el conflicto.
7. Organizan los issues en un tablero de GitHub Projects.

Entrega: link del repositorio del equipo.

## Comandos clave

Desde la carpeta del repositorio, actualiza `main` y crea tu rama. Cambia `samuel` por tu nombre.

```bash
git switch main
git pull --ff-only origin main
git switch -c feat/samuel
```

Después de editar `index.html`, guarda y sube el cambio.

```bash
git add index.html
git commit -m "feat: agregar mi sección de presentación"
git push -u origin feat/samuel
```

## Después del merge

```bash
git switch main
git pull origin main
```
