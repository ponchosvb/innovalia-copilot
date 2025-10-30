# 🚀 Innovalia - Presentación GitHub Copilot

Una aplicación web de una sola página diseñada para mostrar el impacto y beneficios de GitHub Copilot en el desarrollo de software en Innovalia.

## ✨ Características

- **🎨 Diseño moderno**: Interfaz atractiva con Tailwind CSS
- **📊 Visualizaciones interactivas**: Gráficas con Chart.js mostrando KPIs reales
- **⌨️ Efecto de tecleo**: Simulación del comportamiento de Copilot en tiempo real
- **📱 Responsive**: Optimizado para todos los dispositivos
- **🔧 Demo interactivo**: Sección donde los usuarios pueden probar prompts
- **🚀 100% estático**: Perfecto para GitHub Pages, sin necesidad de backend

## 🏗️ Estructura del Sitio

### Secciones incluidas:

1. **🏠 Inicio (Hero)**: Presentación principal con animación de tecleo
2. **⚖️ Antes/Después**: Comparación del desarrollo con y sin Copilot
3. **💼 Casos Reales**: Proyectos exitosos implementados con Copilot
4. **📈 Impacto (KPIs)**: Métricas y gráficas del rendimiento mejorado
5. **🎮 Demo Interactivo**: Simulador de prompts de Copilot
6. **🎯 Créditos**: Reconocimientos y tecnologías utilizadas

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **Tailwind CSS**: Framework de CSS via CDN
- **Vanilla JavaScript**: Funcionalidades interactivas
- **Chart.js**: Visualizaciones de datos
- **Font Awesome**: Iconografía
- **Google Fonts**: Tipografía moderna

## 📋 Instalación y Uso

### Opción 1: Uso directo
1. Descarga o clona este repositorio
2. Abre `index.html` en tu navegador web
3. ¡Listo! El sitio funciona completamente sin servidor

### Opción 2: Desarrollo local con servidor
```bash
# Si tienes Python instalado
python -m http.server 8000

# Si tienes Node.js instalado
npx serve .

# Si tienes PHP instalado
php -S localhost:8000
```

## 🚀 Despliegue en GitHub Pages

### Pasos para publicar:

1. **Crear repositorio en GitHub**
   ```bash
   git init
   git add .
   git commit -m "Inicial: Sitio web Innovalia Copilot"
   git remote add origin https://github.com/tu-usuario/innovalia-copilot.git
   git push -u origin main
   ```

2. **Activar GitHub Pages**
   - Ve a Settings → Pages en tu repositorio
   - En "Source", selecciona "Deploy from a branch"
   - Elige "main" y "/ (root)"
   - Haz clic en "Save"

3. **Acceder al sitio**
   - Tu sitio estará disponible en: `https://tu-usuario.github.io/innovalia-copilot`
   - La publicación puede tardar unos minutos

### Configuración automática
Si quieres automatizar el despliegue, puedes usar GitHub Actions. Crea `.github/workflows/deploy.yml`:

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
    
    - name: Deploy to GitHub Pages
      uses: peaceiris/actions-gh-pages@v3
      with:
        github_token: ${{ secrets.GITHUB_TOKEN }}
        publish_dir: .
```

## 🎨 Personalización

### Datos editables en el código:

#### KPIs (líneas 280-298):
```html
<div class="text-3xl font-bold text-gray-900 mb-2">62%</div>
<div class="text-gray-600">Reducción en tiempo</div>
```

#### Gráficas (líneas 450-480):
```javascript
datasets: [{
    label: 'Con Copilot',
    data: [85, 92, 98, 105, 110, 115], // ← Cambia estos valores
    // ...
}]
```

#### Casos de éxito (líneas 180-260):
```html
<p><strong>Resultado:</strong> 60% menos tiempo de desarrollo</p>
```

### Colores del tema:
El sitio usa la paleta de Tailwind CSS. Para cambiar colores principales:
- **Azul**: `blue-600`, `blue-500`
- **Verde**: `green-600`, `green-500`
- **Púrpura**: `purple-600`, `purple-500`

## 📊 Métricas incluidas

### KPIs mostrados:
- ⏱️ **62%** reducción en tiempo de desarrollo
- 🐛 **45%** menos bugs en producción
- 💻 **80%** de código generado automáticamente
- 😊 **95%** de satisfacción del equipo

### Gráficas:
1. **Productividad por Sprint**: Comparación antes/después de Copilot
2. **Distribución de tareas**: Tiempo invertido por actividad

## 🔧 Funcionalidades JavaScript

### Animaciones incluidas:
- **Typing effect**: Simula escritura de Copilot en hero
- **Smooth scrolling**: Navegación suave entre secciones
- **Card hover effects**: Efectos visuales en tarjetas
- **Demo interactivo**: Simulador de respuestas de Copilot

### Demo de prompts:
El demo responde a palabras clave como:
- "validar email" → Función de validación
- "ordenar array" → Función de ordenamiento
- "fecha actual" → Función de fecha
- Cualquier otro prompt → Función genérica

## 📁 Estructura de archivos

```
innovalia-copilot/
├── index.html          # Archivo principal (todo el sitio)
├── README.md           # Este archivo
└── .github/
    └── workflows/
        └── deploy.yml  # (Opcional) GitHub Actions
```

## 🌟 Características destacadas

### Responsive Design
- **Mobile-first**: Optimizado para móviles
- **Breakpoints**: sm, md, lg, xl de Tailwind
- **Navegación móvil**: Menú hamburguesa incluido

### Performance
- **CDN loading**: Todas las librerías via CDN
- **Optimized images**: Solo iconos SVG/Font
- **Minimal JS**: JavaScript vanilla sin frameworks pesados

### SEO Optimizado
- **Meta tags**: Descripción y título optimizados
- **Semantic HTML**: Estructura semántica correcta
- **Alt texts**: Textos alternativos en iconos

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-seccion`)
3. Commit tus cambios (`git commit -m 'Agregar nueva sección'`)
4. Push a la rama (`git push origin feature/nueva-seccion`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 📞 Contacto

**Innovalia**
- 🌐 Website: [https://tu-usuario.github.io/innovalia-copilot](https://tu-usuario.github.io/innovalia-copilot)
- 📧 Email: contacto@innovalia.com
- 🐙 GitHub: [@tu-usuario](https://github.com/tu-usuario)

---

⭐ **¡Dale una estrella al repositorio si te gusta el proyecto!** ⭐

*Presentación creada con GitHub Copilot para demostrar su capacidad real en desarrollo web.*