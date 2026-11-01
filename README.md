# BCA - Maqueta web del banco (HTML + CSS)

Proyecto académico. Solo HTML5 y CSS3: sin JavaScript ni backend.

## Estructura

```
BCA/
├── index.html                  (Byron)
├── pages/
│   ├── _plantilla.html         (copiar para crear cada página)
│   ├── nosotros.html           (Byron)
│   └── ...                     (resto de páginas del equipo)
├── css/
│   ├── variables.css           (Byron: colores, fuentes, espacios)
│   ├── global.css              (Byron: base y botones .btn)
│   ├── components/
│   │   ├── header.css          (Byron: navbar)
│   │   └── footer.css          (Byron: footer)
│   ├── home.css                (Byron)
│   ├── nosotros.css            (Byron)
│   └── ...                     (un CSS propio por página)
└── img/                        (imágenes; cada quien en su subcarpeta)
```

## Cómo empezar (todos)

1. Clonen el repo y creen su rama: `git checkout -b feature/tu-nombre`
2. Copien `pages/_plantilla.html`, renómbrenla con el nombre acordado (ej. `login.html`).
3. Creen su CSS en `css/` y cámbienlo en el último `<link>` del `<head>`.
4. Escriban su contenido **solo dentro de `<main>`**. No modifiquen navbar, footer ni los CSS de Byron.
5. En el navbar de su página marquen su enlace con `aria-current="page"` (se resalta solo).

## Reglas

- Orden de CSS: `variables > global > header > footer > tu CSS`.
- Usen los colores y fuentes con `var(--...)` (ver `css/variables.css`). No inventen colores sueltos.
- Botones listos: `.btn` + `.btn-primario`, `.btn-acento`, `.btn-borde`.
- Contenedor centrado: `.contenedor`. Sección con espacio vertical: `.seccion`.
- Prefijo propio en sus clases (`.login-`, `.cuentas-`, `.prestamo-`, `.contacto-`...) para que no choquen.
- Cada quien toca únicamente sus archivos. Pull request a `main` al terminar.

## Nombres de archivo acordados

| Página | HTML | CSS |
|---|---|---|
| Cuentas y tarjetas | pages/cuentas-tarjetas.html | css/cuentas-tarjetas.css |
| Inversiones / ahorros | pages/inversiones-ahorros.html | css/inversiones-ahorros.css |
| Login | pages/login.html | css/login.css |
| Transferencia | pages/transferencia.html | css/transferencia.css |
| Préstamos | pages/prestamos.html | css/prestamos.css |
| Beneficios / puntos | pages/beneficios-puntos.html | css/beneficios-puntos.css |
| Contacto | pages/contacto.html | css/contacto.css |
| Sucursales | pages/sucursales.html | css/sucursales.css |
| FAQ | pages/faq.html | css/faq.css |

El navbar y el footer ya enlazan a estos nombres exactos.

## Subir la base a GitHub (Byron)

```
cd BCA
git init
git add .
git commit -m "Base del proyecto: plantilla, navbar, footer, inicio y nosotros"
git branch -M main
git remote add origin https://github.com/USUARIO/REPO.git
git push -u origin main
```
