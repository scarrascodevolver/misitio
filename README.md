# Portfolio Elías Carrasco Aguayo

Portfolio web profesional desarrollado con HTML5 + TailwindCSS.

## 🎨 Dos Diseños Disponibles

### **index.html** - Diseño Glassmorphism Moderno
- Fondo oscuro con gradientes purple/indigo
- Efectos glass/blur elegantes
- Colores suaves: Indigo, Purple, Pink, Green, Orange
- Animaciones floating suaves
- Ideal para: Portfolio profesional elegante

### **index-v2.html** - Diseño Cyberpunk/Neon
- Fondo negro con grid futurista
- Efectos neón brillantes
- Colores vibrantes: Verde Neón, Cyan, Magenta, Yellow
- Estilo código/sintaxis
- Ideal para: Desarrollador con estilo tech/hacker

## 🚀 Cómo usar

### 1. Agregar tus videos
Coloca tus videos de proyectos en la carpeta `assets/videos/` con los nombres:
- `proyecto1.mp4` - Sistema de Solicitud de Insumos
- `proyecto2.mp4` - Sistema de Enumeración de Planos
- `proyecto3.mp4` - Sistema de Análisis de Video Deportivo
- `proyecto4.mp4` - Aplicaciones Web Empresariales

**Recomendaciones para videos:**
- Formato: MP4 (H.264)
- Duración: 30-60 segundos
- Resolución: 720p o 1080p
- Peso: Máximo 10MB por video (para carga rápida)

### 2. Abrir el sitio
Con XAMPP corriendo, abre en tu navegador:

**Versión 1 (Glassmorphism):**
```
http://localhost/sitio/
```

**Versión 2 (Cyberpunk):**
```
http://localhost/sitio/index-v2.html
```

### 3. Personalizar enlaces
Edita en `index.html` e `index-v2.html` estos enlaces:
- LinkedIn: Reemplaza `https://www.linkedin.com/in/sergio-carrasco` con tu URL real
- GitHub: Reemplaza `https://github.com/sergiocarrasco` con tu usuario real
- Email: Verifica que `eliascarrascoaguayo@gmail.com` sea correcto

## 🎨 Cambiar diseño/colores

### Cambiar colores principales
En la línea 8-9 de `index.html`:
```javascript
colors: {
    primary: '#2563eb',    // Azul principal - cámbialo por otro color hex
    secondary: '#1e40af',  // Azul secundario
}
```

**Ejemplos de paletas:**
- Verde: `primary: '#059669'`, `secondary: '#047857'`
- Morado: `primary: '#7c3aed'`, `secondary: '#6d28d9'`
- Rojo: `primary: '#dc2626'`, `secondary: '#b91c1c'`

### Cambiar foto de perfil
Actualmente hay un círculo con "SC". Para poner tu foto:
1. Guarda tu foto en `assets/foto-perfil.jpg`
2. Reemplaza las líneas 74-76 por:
```html
<div class="md:w-1/2 flex justify-center">
    <img src="assets/foto-perfil.jpg" alt="Sergio Carrasco"
         class="w-64 h-64 rounded-full shadow-2xl object-cover">
</div>
```

## 📱 Vista previa
El sitio es 100% responsive (se adapta a móviles, tablets y desktop).

## 🔧 Próximos pasos

### Para publicar en .es o .com:
1. **Comprar dominio:** GoDaddy, Namecheap, Hostinger (~10€/año)
2. **Hosting:**
   - Compartido: Hostinger, SiteGround (~3-5€/mes)
   - VPS: DigitalOcean, Vultr (~5€/mes) - ya tienes experiencia con esto
3. **Subir archivos:** Por FTP o Git

### Optimizar antes de publicar:
- Comprimir videos (usa HandBrake)
- Optimizar imágenes (TinyPNG)
- Probar en diferentes navegadores

## 💡 Ideas para iterar

### Versión 2 - Agregar:
- Formulario de contacto funcional
- Botón de descarga de CV en PDF
- Animaciones al hacer scroll
- Modo oscuro/claro

### Versión 3 - Backend Laravel:
- Panel admin para subir proyectos
- Blog técnico
- Estadísticas de visitas

## 📞 Estructura actual
```
sitio/
├── index.html          # Página principal
├── assets/
│   └── videos/        # Coloca aquí tus videos .mp4
└── README.md          # Este archivo
```

---

**Stack:** HTML5 + TailwindCSS CDN + Vanilla JavaScript
**Sin dependencias** - Listo para desplegar en cualquier servidor web
