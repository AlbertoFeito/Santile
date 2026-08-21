# Notas para Claude en este repositorio

Este archivo es contexto persistente para cualquier sesión de Claude que trabaje en
Santilé más adelante. Léelo antes de tocar nada — evita repetir trabajo o deshacer
decisiones ya tomadas con el cliente.

## Qué es Santilé

E-commerce de venta de cajas de productos (no unidades sueltas) para la comunidad
espirituana/cubana en el exterior. Categorías: Cárnicos, Alimentos, Aceite y
Condimentos, Dulces, Galletas. El cliente (Santana) ya vendía por WhatsApp con
anuncios estilo tarjeta (ver `docs/assets/anuncio-*.jpg`) — esa estética de marca
(azul marino, blanco, sellos de "Calidad Premium", formato "Caja x N unidades") es
la que define el diseño, no algo libre a reinterpretar.

## Fuente de verdad

`index.html` en la raíz es la maqueta aceptada por el cliente. Es un único archivo
autocontenido (HTML + CSS + JS, sin build, sin dependencias) que se puede abrir con
doble clic. **No crear versiones paralelas** (`demo.html`, `index-pro.html`,
`ecommerce-full.html`, etc.) — si hay que explorar una alternativa de diseño, se
prueba directamente en `index.html` o en una rama, se muestra al cliente, y solo si
se aprueba se integra. La historia de este repo ya tuvo el problema de que varias
sesiones generaron implementaciones distintas en paralelo y eso generó confusión
sobre cuál era la válida — el commit `519299b` en `main` resolvió eso adoptando
esta maqueta como única fuente de verdad. Las implementaciones descartadas siguen
en el historial de git por si hace falta rescatar algo, pero no son el punto de
partida para seguir trabajando.

## Estado del proyecto

- **Front-end**: maqueta funcional con datos hardcodeados (catálogo, precios,
  direcciones de ejemplo). Todo el estado del carrito/usuario/pedidos vive en
  `localStorage` del navegador, no hay servidor.
- **Backend**: no existe todavía. Es la siguiente fase.
- **Stack actual**: HTML/CSS/JS vanilla en un solo archivo, sin build. Es
  deliberado mientras se valida el diseño con el cliente — permite compartir el
  archivo o un enlace de vista previa al instante, sin instalar nada.
- **Stack futuro**: cuando arranque el backend, migrar a Next.js (páginas/rutas de
  API, mejor organización en componentes, más fácil de mantener entre varios
  colaboradores). No migrar antes de que el diseño esté aprobado — perdería la
  ventaja de "ábrelo y ya" que tiene ahora mismo.

## Flujo que el cliente pidió explícitamente

1. Catálogo por categoría, todo vendido **por caja**, nunca por unidad suelta.
2. Carrito: +/- por producto, total de compra visible antes del botón de
   finalizar.
3. Checkout en 3 pasos: datos de quien recibe (elegir dirección guardada del
   perfil o introducir una nueva) → pago → confirmación.
4. Sesión de usuario con funcionalidades básicas (direcciones guardadas,
   historial de pedidos).

Si se agregan pasos o se cambia este flujo, confirmarlo con el cliente primero —
fue una especificación explícita, no una suposición de diseño.

## Convenciones

- Todo el contenido visible (textos, commits en el PR/README) va en español,
  igual que la comunicación con el cliente.
- Los assets de marca y las capturas de referencia viven en `docs/assets/`.
- Antes de dar por bueno un cambio de layout, probarlo en un viewport angosto
  real (320–390px), no solo en escritorio — el repo ya tuvo un bug de
  desbordamiento horizontal en móvil que no se notaba en capturas de escritorio.
