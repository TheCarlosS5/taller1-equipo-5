# Estándar de codificación - Equipo 5

Lenguaje(s) del proyecto formativo: PHP, HTML, CSS, JavaScript y SQL (MySQL)

## 1. Nombrado
(pendiente)

## 2. Formato
(pendiente)

## 3. Comentarios y documentación
(pendiente)

## 4. Estructura de carpetas

```text
la-unica/
├── assets/               # Recursos estáticos del frontend
│   ├── css/              # Hojas de estilo
│   ├── fonts/            # Tipografías
│   ├── img/              # Imágenes e íconos
│   ├── js/               # Scripts de JavaScript
│   └── video/            # Videos
├── php/                  # Lógica y vistas PHP organizadas por módulo
│   ├── config/           # Conexión a BD y configuración
│   ├── includes/         # Componentes reutilizables (header, footer)
│   ├── inicio/           # Pantalla principal / dashboard
│   ├── clientes/         # Gestión de clientes
│   ├── productos/        # Gestión de productos
│   ├── facturas/         # Facturación
│   ├── historial/        # Historial de movimientos
│   ├── reportes/         # Reportes del sistema
│   └── sobre_nosotros/   # Información del proyecto
├── logs/                 # Registros de errores y eventos
├── tests/                # Pruebas técnicas y de seguridad
├── wiki/                 # Documentación web interna
├── referencias/          # Documentos (SRS, PAC, manuales, MER y scripts SQL)
├── index.php             # Punto de entrada
├── main.php              # Vista principal
├── .htaccess             # Reglas de Apache
├── .gitignore            # Archivos excluidos de Git
└── README.md             # Documentación principal
```

**Reglas:**
- Cada módulo nuevo va en su propia carpeta dentro de `php/`.
- Todo archivo CSS, JS o imagen va en `assets/`, no dentro de `php/`.
- Los scripts SQL y documentos del proyecto se guardan en `referencias/`.
- No dejar archivos temporales o pruebas sueltas en la raíz.

## 5. Git: ramas, commits y pull requests
(pendiente)