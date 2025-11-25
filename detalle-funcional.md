# Detalle Funcional de MasterPC

## **Funcionalidades Detalladas del Sistema**

### **Módulo de Tienda Online**

**Catálogo de productos** con las siguientes características:
- *Filtrado avanzado* por categorías (componentes, ordenadores, móviles, accesorios)
- **Búsqueda en tiempo real** con sugerencias
- Vista en cuadrícula y lista
- Paginación de resultados (20 productos por página)

**Sistema de carrito de compras**:
- Almacenamiento en `localStorage` del navegador
- Actualización en tiempo real del total
- Cálculo automático de gastos de envío
- *Persistencia* entre sesiones

### **Módulo de Servicio Técnico**

**Formulario inteligente de solicitud** que incluye:
- **Validación en tiempo real** de campos obligatorios
- Selección de tipo de servicio (reparación, mantenimiento, mejora)
- Subida de imágenes del equipo (máximo 3 archivos, 5MB cada uno)
- *Estimación automática* de costo y tiempo aproximado

### **Flujo de Usuario Principal**

1. **Navegación y búsqueda**
   - Usuario accede al catálogo
   - Filtra por categoría y precio
   - Visualiza detalles del producto

2. **Gestión del carrito**
   - Añade productos al carrito
   - Modifica cantidades
   - Procede al checkout

3. **Solicitud de servicio técnico**
   - Completa formulario paso a paso
   - Sube evidencias del equipo
   - Recibe confirmación por email

## **Tipos de Usuarios y Permisos**

| Tipo de Usuario | Funcionalidades Específicas | Accesos |
|-----------------|-----------------------------|---------|
| **Invitado** | Ver catálogo, filtrar productos | Lectura básica |
| **Cliente Registrado** | Compra online, historial pedidos, solicitar servicio | Lectura/Escritura limitada |
| **Técnico** | Gestionar solicitudes, actualizar estados, subir reportes | Módulo técnico completo |
| **Administrador** | Gestionar productos, usuarios, reportes | Acceso total al sistema |

## **Especificaciones Técnicas Avanzadas**

### **Frontend - Estructura de Componentes**

```html
<!-- Ejemplo de tarjeta de producto -->
<div class="product-card">
    <img src="images/products/rtx-4080.jpg" alt="RTX 4080">
    <h3>GeForce RTX 4080</h3>
    <p class="price">$899.00</p>
    <button class="add-to-cart" data-product-id="123">
        Añadir al Carrito
    </button>
</div>
