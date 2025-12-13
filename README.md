# Miguel Systems – Proyecto Intermodular

Este proyecto consiste en el desarrollo de la web corporativa de **Miguel Systems**, una consultora tecnológica especializada en soluciones digitales, desarrollo web y servicios cloud.  


##  Decisiones de diseño

### **Colores**
Se ha utilizado una paleta basada en tonos azules:
- Azul primario: #0056ff  
- Azul oscuro: #003bbd  
- Grises suaves para fondos y tarjetas  

El azul transmite confianza, tecnología y profesionalidad, valores asociados a la marca.

### **Tipografía**
Se ha utilizado **Montserrat** (Google Fonts) por su legibilidad y estética moderna.  
Se aplica globalmente para mantener coherencia visual.

### **Estructura**
El sitio sigue una estructura semántica clara:
- `<header>` con logo y navegación  
- `<main>` dividido en secciones  
- `<footer>` con información legal  
- Navegación consistente en todas las páginas  

La página del proyecto incluye un **layout de dos columnas (main + aside)** y una tabla informativa con estilo zebra.

---

## Técnicas utilizadas

### **Flexbox**
- Menú de navegación  
- Hero centrado vertical y horizontalmente  
- Galería de servicios con `flex-wrap`  
- Layout del proyecto (main + aside)

### **CSS Grid**
- Sección de beneficios (bonus)

### **Responsive Design**
- Breakpoint principal a 768px  
- Menú móvil  
- Columnas que colapsan a una sola  
- Galería adaptada a pantallas pequeñas  

Incluye el comentario obligatorio en el media query.

### **Formulario conectado al backend**
El formulario utiliza:
- `action="https://morning-paper-a0fc.contry-1990.workers.dev"`  
- `method="POST"`  
- Campos con `name` obligatorios  
- Validación HTML5 (`required`, `type="email"`, `minlength`)  
- Estados visuales `:focus`, `:valid`, `:invalid`

### **Tabla con zebra**
La tabla del proyecto usa `nth-child(even)` para filas alternas.

---

##  Dificultades encontradas y soluciones

### **1. Menú responsive**
**Problema:** El menú se superponía en móvil.  
**Solución:** Implementar un botón hamburguesa y cambiar `flex-direction` a columna en el breakpoint.

### **2. Layout del proyecto**
**Problema:** El aside no se adaptaba bien en pantallas pequeñas.  
**Solución:** Añadir `flex-direction: column` en el media query.

### **3. Formulario funcional**
**Problema:** El backend requería nombres específicos y validación.  
**Solución:** Añadir atributos `name`, `action`, `method` y validación HTML5.

### **4. Galería de servicios**
**Problema:** Inicialmente estaba hecha con Grid, pero la rúbrica pedía Flexbox.  
**Solución:** Reescribirla con `display: flex` y `flex-wrap: wrap`.

---

##  Conclusión

El proyecto cumple los requisitos del módulo:
- HTML semántico  
- CSS moderno  
- Flexbox + Grid  
- Responsive  
- Formulario funcional  
- Tabla, aside, hero, navegación  
- Diseño profesional y coherente  

