# taller-1

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

## Despues del merge

```bash
git switch main
git pull origin main
```
