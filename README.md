# Equipo 5 - los hijos de Elon Musk

## Descripción

Taller 1 del Equipo 5 sobre Git y GitHub. El proyecto incluye una página HTML de ejemplo y las fichas de presentación del equipo. El taller sirve para practicar el trabajo colaborativo con ramas, issues, pull requests y resolución de conflictos.

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
3. Cada uno clona el repo y crea su propia rama.
4. Commit y push de la rama; abre un PR con "Closes #n".
5. Otro compañero revisa, comenta y aprueba; luego merge.
6. Dos integrantes editan la misma línea y resuelven el conflicto.
7. Organizan los issues en un tablero de GitHub Projects.

Entrega: link del repositorio del equipo.

## Comandos clave

```bash
git clone <url-del-repo>
git switch -c feature/mi-seccion
git add .
git commit -m "feat: mi seccion"
git push -u origin feature/mi-seccion
```

## Después del merge

```bash
git switch main
git pull origin main
```

Consulta nuestro [estándar de codificación](ESTANDAR.md).

