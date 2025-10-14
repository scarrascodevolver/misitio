# 📋 Instrucciones para Actualizar Landing Pages

## ✅ Lo que se implementó:

1. **Sistema de filtros** con 3 categorías:
   - `[TODOS]` - Muestra todos los proyectos
   - `[SISTEMAS_WEB]` - Solo sistemas Laravel
   - `[LANDING_PAGES]` - Solo landing pages

2. **6 Landing Pages placeholder** listas para personalizar

3. **Diseño responsive** adaptado al estilo cyberpunk/neon

---

## 🔧 Cómo reemplazar las imágenes:

### Paso 1: Captura screenshots de tus landing pages

**Opción fácil:**
- Windows: `Win + Shift + S`
- Mac: `Cmd + Shift + 4`
- Extensión Chrome: "GoFullPage" (captura completa con scroll)

**Opción profesional (mockups):**
- https://screely.com - Agrega fondos/sombras automáticamente
- https://mockuper.net - Mockups en dispositivos
- https://shots.so - Mockups minimalistas

### Paso 2: Optimiza las imágenes

**Especificaciones recomendadas:**
- Ancho: 600-800px
- Formato: JPG (80-90% calidad) o WebP
- Peso: < 200KB por imagen

**Herramientas:**
- https://tinypng.com - Compresión automática
- https://squoosh.app - Optimización avanzada

### Paso 3: Guarda las imágenes

Crea la carpeta (si no existe):
```
/assets/img/
```

Nombra tus archivos:
```
landing-1.jpg
landing-2.jpg
landing-3.jpg
landing-4.jpg
landing-5.jpg
landing-6.jpg
```

### Paso 4: Reemplaza en index-v2.html

Busca los comentarios `🔔 REEMPLAZA` en el archivo y actualiza:

**Imagen:**
```html
<!-- ANTES -->
<img src="https://via.placeholder.com/600x400/667eea/ffffff?text=Landing+Page+1"

<!-- DESPUÉS -->
<img src="assets/img/landing-1.jpg"
```

**Enlace al sitio:**
```html
<!-- ANTES -->
<a href="#" target="_blank"

<!-- DESPUÉS -->
<a href="https://tu-sitio-real.com" target="_blank"
```

**Título y descripción:**
```html
<!-- Personaliza -->
<h3>Tu Título Real</h3>
<p>Tu descripción real del proyecto...</p>
```

**Tags de tecnologías:**
```html
<!-- Personaliza según lo que usaste -->
<span class="text-yellow">#HTML</span>
<span class="text-cyan">#CSS</span>
<span class="text-magenta">#jQuery</span>
```

---

## 📍 Ubicaciones exactas en index-v2.html:

| Landing | Línea aprox. | Imagen                | Enlace        |
|---------|--------------|----------------------|---------------|
| 1       | ~262         | `assets/img/landing-1.jpg` | línea ~269    |
| 2       | ~299         | `assets/img/landing-2.jpg` | línea ~305    |
| 3       | ~335         | `assets/img/landing-3.jpg` | línea ~341    |
| 4       | ~371         | `assets/img/landing-4.jpg` | línea ~377    |
| 5       | ~407         | `assets/img/landing-5.jpg` | línea ~413    |
| 6       | ~443         | `assets/img/landing-6.jpg` | línea ~449    |

Busca el comentario: `<!-- 🔔 REEMPLAZA`

---

## 🎨 Personalización adicional:

### Cambiar cantidad de landing pages:

**Agregar más:**
1. Copia cualquier bloque `<!-- Landing X -->`
2. Cambia el número `[0X]`
3. Actualiza imagen, enlace y contenido

**Eliminar:**
1. Borra todo el bloque `<div class="project-card" data-category="landing">...</div>`

### Cambiar colores de badges:

Los colores cyberpunk disponibles:
- `text-neon` / `border-neon` - Verde neón
- `text-cyan` / `border-cyan` - Cyan
- `text-magenta` / `border-magenta` - Magenta
- `text-yellow` / `border-yellow` - Amarillo

---

## ✨ Resultado final:

- ✅ Filtros funcionales con animaciones
- ✅ 2 Sistemas Web + 6 Landing Pages
- ✅ Hover interactivo con botón "VER_SITIO"
- ✅ Diseño responsive (móvil/tablet/desktop)
- ✅ Estilo cyberpunk coherente

---

## 🆘 Problemas comunes:

**Las imágenes no se ven:**
- Verifica que la ruta sea correcta: `assets/img/landing-X.jpg`
- Verifica que la carpeta `assets/img/` exista
- Verifica que el nombre del archivo coincida exactamente

**Los filtros no funcionan:**
- Asegúrate de que cada card tenga `data-category="landing"` o `data-category="sistemas"`
- Verifica que el JavaScript esté al final del HTML (antes de `</body>`)

**El diseño se ve mal:**
- No elimines las clases de Tailwind CSS
- Mantén la estructura de grid: `grid md:grid-cols-2 lg:grid-cols-3`

---

¿Necesitas ayuda? Busca los comentarios `🔔` en index-v2.html
