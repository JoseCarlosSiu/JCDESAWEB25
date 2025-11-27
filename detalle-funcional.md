# Detalle Funcional de MasterPC

## **Funcionalidades Detalladas del Sistema**

### **Módulo de Tienda Online**

**Catálogo de productos** con las siguientes características:
- *Filtrado avanzado* por categorías (componentes, ordenadores, móviles, accesorios)
- **Búsqueda en tiempo real** con sugerencias(depende como vaya con javascript)
- Vista en cuadrícula y lista
- Paginación de resultados (5 productos por página depende como lo vea)

**Sistema de carrito de compras**:
- Almacenamiento para que este cuando te salga y tal
- Actualización en tiempo real del total
- Cálculo automático de gastos de envío
- *Persistencia* entre sesiones

### **Módulo de Servicio Técnico**

**Formulario para las solicitudes** que incluye:
- **Validación en tiempo real** de campos obligatorios
- Selección de tipo de servicio (reparación, mantenimiento, mejora)
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
   - Recibe confirmación por email (hay una pagina para eso)

## **Tipos de Usuarios y Permisos**

| Tipo de Usuario | Funcionalidades Específicas | Accesos |
|-----------------|-----------------------------|---------|
| **Invitado** | Ver catálogo, filtrar productos | Lectura básica |
| **Cliente Registrado** | Compra online, historial pedidos, solicitar servicio | Lectura/Escritura limitada |
| **Técnico** | Gestionar solicitudes, actualizar estados, subir reportes | Módulo técnico completo |
| **Administrador** | Gestionar productos, usuarios, reportes | Acceso total al sistema |

## **Especificaciones Técnicas Avanzadas**

### **Frontend - Estructura de Componentes**
<!--por ejemplo aqui puse uno por ejemplo de mi pagina web creada -->
```html
<!-- Ejemplo de tarjeta de producto -->
<div class="product-card">
    <img src="images/products/rtx-5090.jpg" alt="RTX 5090">
    <h3>GeForce RTX 5090</h3>
    <p class="price">$1599.00</p>
    <button class="add-to-cart" data-product-id="123">
        Añadir al Carrito
    </button>
</div>
```
[Volver a README.md](./README.md)
