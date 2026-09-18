# Sesión 17 — Bootstrap: introducción al framework

**Fecha de entrega:** 18 de septiembre de 2026
**Nombres y apellidos:** Mateo Rave Girlado
**Número de ficha:** 3267541
**Competencia:** Crear Componentes Front-End del Software
**Instructor:** Alexander Patiño

## Descripción

Landing page de **FluneXy** (aplicación de finanzas personales) construida en un único `index.html`, usando exclusivamente clases de Bootstrap 5 cargado por CDN — sin una sola línea de CSS propio.

## Secciones

- **Hero:** grid de 2 columnas en escritorio (`col-12 col-lg-6`) — titular, texto y botones a la izquierda, imagen a la derecha; apiladas en una sola columna en móvil.
- **Características:** 3 cards en fila (`col-12 col-md-6 col-lg-4`) — apiladas en móvil, 2 por fila en tablet, 3 por fila en escritorio.
- **Llamada a la acción:** sección `bg-primary` con un botón `btn btn-light`.
- **Footer:** `bg-dark`, centrado, con el nombre del proyecto y el crédito académico.

## Cómo cumple los criterios de evaluación

1. **Grid responsive:** todas las columnas parten de `col-12` (base móvil) y escalan con `col-md-*` (cards) y `col-lg-*` (hero y cards).
2. **Viewport + CDN oficial:** `<meta name="viewport">` está presente y Bootstrap 5.3.3 se carga desde `cdn.jsdelivr.net` con `integrity` y `crossorigin`.
3. **Espaciado solo con utilidades:** todo el espaciado usa clases `py-*`, `p-*`, `mb-*`, `me-*`, `g-*` — no hay ningún `style=""` con píxeles.
4. **Colores semánticos:** `bg-dark`, `bg-primary`, `bg-primary-subtle`, `text-white`, `text-white-50`, `text-body-secondary`, etc. — ningún color está escrito a mano.
5. **Sin scroll horizontal en 375px:** todas las filas están dentro de un `container`, y la imagen del hero usa `img-fluid` para nunca desbordar su columna. Verificado con un navegador automatizado a 375px de ancho.

## Cómo probarlo

1. Clonar o descargar el repositorio.
2. Abrir `index.html` en el navegador (requiere conexión a internet, porque Bootstrap se carga desde el CDN).
3. Reducir el ancho de la ventana (o abrir las herramientas de desarrollador en modo responsive a 375px) para comprobar que el layout se adapta sin scroll horizontal.
