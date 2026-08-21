# Santilé — E-commerce Premium de Productos Locales

Plataforma de e-commerce moderna para vender **cajas de productos locales premium** con entrega a domicilio.

## 🎯 Sobre el Proyecto

Santilé es una tienda online funcional que permite:
- 🛍️ Explorar 50+ productos en 5 categorías
- 🛒 Carrito dinámico con gestión de cantidades  
- 💳 Checkout completo con formulario de datos
- 👤 Gestión de cuenta y historial de órdenes
- ❤️ Sistema de favoritos/wishlist
- 📱 Experiencia mobile-first responsiva
- 🌙 Tema claro/oscuro automático

## 📂 Archivos Disponibles

### **Demostraciones**
- **`ecommerce-full.html`** ⭐ **RECOMENDADO** - Versión completa con todas las secciones
- `index-pro.html` - Versión profesional optimizada
- `demo.html` - Versión funcional mejorada
- `index.html` - Versión original con SPA completo

### **Configuración**
- `vercel.json` - Config para despliegue en Vercel
- `.github/workflows/deploy.yml` - CI/CD para GitHub Pages
- `README.md` - Este archivo

## 🚀 Cómo Usar

### Opción 1: Abrir Localmente
1. Descarga `ecommerce-full.html`
2. Abre en navegador (doble click)
3. ¡Funciona offline, sin servidor necesario!

### Opción 2: Desplegar en Producción
```bash
# GitHub Pages
1. Habilita en Settings → Pages → GitHub Actions

# O Vercel
1. Conecta el repo en vercel.com
2. Vercel detecta vercel.json automáticamente
3. Deploy automático en cada push
```

## 🛒 Funcionalidades Principales

### **Tienda**
- ✅ 50 productos en 5 categorías (Cárnicos, Alimentos, Aceite, Dulces, Galletas)
- ✅ Búsqueda en tiempo real
- ✅ Filtros por categoría
- ✅ Vista de producto detallado
- ✅ Sistema de favoritos persistente

### **Carrito & Compras**
- ✅ Carrito lateral dinámico
- ✅ Agregar/quitar/modificar cantidad
- ✅ Total automático
- ✅ Checkout con validación
- ✅ Historial de órdenes guardado

### **Cuenta de Usuario**
- ✅ Perfil de usuario
- ✅ Historial completo de compras
- ✅ Estado de órdenes
- ✅ Información de contacto

### **Soporte**
- ✅ 5 FAQs expandibles
- ✅ Formulario de contacto funcional
- ✅ Centro de ayuda

## 💾 Tecnología

```
Frontend:
  - HTML5 semántico
  - CSS3 (Grid, Flexbox, Variables CSS)
  - JavaScript vanilla (SPA, localStorage)
  
Design:
  - Tipografía: Playfair Display + Outfit (Google Fonts)
  - Colores: Paleta profesional dorado/marrón
  - Responsive: Mobile-first, Tablet & Desktop
  - Tema: Claro/Oscuro automático
  
Persistencia:
  - localStorage para carrito, wishlist, órdenes
  - Funciona offline completamente
```

## 🎨 Características de Diseño

- 📱 **Responsive Completo**: Funciona perfectamente en mobile, tablet y desktop
- 🌙 **Tema Dual**: Detecta preferencia del sistema automático
- ⚡ **Sin Dependencias**: Vanilla JS, sin frameworks
- 🎯 **UX Profesional**: Animaciones suaves, feedback visual, navegación intuitiva
- ♿ **Accesible**: Semántica HTML correcta, buen contraste

## 📊 Estadísticas del Demo

| Métrica | Valor |
|---------|-------|
| **Productos** | 50 |
| **Categorías** | 5 |
| **Líneas de Código** | ~1,300 |
| **Dependencias Externas** | 0 |
| **Tamaño del Archivo** | ~35KB (sin comprimir) |
| **Tiempo de Carga** | <1s |

## 🔄 Roadmap - Próximos Pasos

### Fase 1: Validación (En Progreso)
- [x] Demo estático funcional
- [x] Todas las páginas del flujo
- [ ] Imágenes reales de productos
- [ ] Integración con sistemas de imagen

### Fase 2: Backend (Pendiente)
- [ ] API Node.js/Python
- [ ] Base de datos (PostgreSQL/MongoDB)
- [ ] Autenticación real
- [ ] Sistema de pagos (Stripe/MercadoPago)

### Fase 3: Producción
- [ ] Admin dashboard
- [ ] Panel de gestión de productos
- [ ] Integración de imágenes CDN
- [ ] Análisis y reportes

## 🎯 Para Colaboradores

Si deseas agregar funcionalidades:

1. **Imágenes de Productos**: Crea una carpeta `/assets/products/` con imágenes para reemplazar los emojis
2. **Backend**: Prepara endpoints en `/api/`
3. **Estilos**: Modifica variables CSS en `:root{}`
4. **Contenido**: Actualiza el objeto `PRODUCTS` en JavaScript

## 📝 Ejemplo de Agregar Imágenes

```html
<!-- Reemplazar: -->
<div class="product-image">🥩</div>

<!-- Con: -->
<div class="product-image">
  <img src="/assets/products/carne-molida.jpg" alt="Carne Molida Premium">
</div>
```

## 🤝 Contribuir

1. Fork el proyecto
2. Crea tu rama (`git checkout -b feature/nueva-funcion`)
3. Commit cambios (`git commit -m 'Add: descripción'`)
4. Push (`git push origin feature/nueva-funcion`)
5. Abre un Pull Request

## 📧 Contacto

- **Email**: info@santile.com
- **Instagram**: @santile.ar
- **WhatsApp**: +54 9 11 XXXX-XXXX

## 📄 Licencia

Proyecto propietario de Santilé © 2024

---

**Creado con ❤️ para promover productos locales premium**