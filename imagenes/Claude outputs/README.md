# 🌏 LOOT CHINO - Catálogo Premium

Catálogo interactivo profesional de productos chinos premium para Loot Chino, desarrollado con HTML5 y CSS3 moderno. Desplegado en Vercel para máxima disponibilidad.

## ✨ Características

- 🎨 **Diseño Profesional**: Paleta de colores exclusiva (Azul oscuro, Dorado, Rojo)
- 🔤 **Tipografías Chinas**: "Ma Shan Zheng" (estilo caligráfico) + "Noto Sans SC" (moderna)
- 📱 **100% Responsivo**: Funciona perfectamente en móvil, tablet y desktop
- ⚡ **Ultra Rápido**: HTML estático, sin dependencias pesadas
- 🎯 **13 Productos**: Todos con imágenes, especificaciones y precios
- 💳 **Listo para Vender**: Mostrar a clientes sin cambios necesarios
- 🚀 **Desplegado en Vercel**: URL compartible en segundos

## 📂 Estructura del Proyecto

```
loot-chino-catalogo/
├── index.html                 # Catálogo principal
├── imagenes/                  # Carpeta de imágenes de productos
│   ├── mochis_fresa.png
│   ├── buldak_carbonara.jpg
│   ├── buldak_spicyhabanero.webp
│   ├── fideos_caldo.png
│   ├── te_herbal_wanglaoji.png
│   ├── te_hierbas_jiduobao.webp
│   ├── bebida_lechecoco.jpeg
│   ├── bebida_naranja_estilo_hong_kong.jpg
│   ├── pocky_berries.webp
│   ├── galletas_naranja.webp
│   ├── galletas_pina.webp
│   ├── pocky_peach.jpg
│   └── polvo_matcha.jpg
├── vercel.json               # Configuración Vercel
├── .gitignore               # Archivos a ignorar en Git
└── README.md                # Este archivo
```

## 🚀 Deployment en Vercel

### Opción 1: Usar Git (Recomendado)

1. **Crear repositorio en GitHub**
   ```bash
   # En tu computadora
   cd ~/Downloads/Loot\ cino
   git init
   git add .
   git commit -m "Initial commit: Loot Chino catalog"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/loot-chino-catalogo.git
   git push -u origin main
   ```

2. **Conectar en Vercel**
   - Ve a [vercel.com](https://vercel.com)
   - Click en "New Project"
   - Importa tu repositorio de GitHub
   - Vercel auto-detectará la configuración
   - Click en "Deploy" ✅

3. **Tu sitio estará en vivo en minutos**
   ```
   https://loot-chino-catalogo.vercel.app
   ```

### Opción 2: Deploy Directo sin Git

1. Descarga [Vercel CLI](https://vercel.com/docs/cli)
   ```bash
   npm install -g vercel
   ```

2. En tu carpeta del proyecto
   ```bash
   vercel
   ```

3. Sigue las instrucciones y confirma el deploy

## 🎨 Paleta de Colores

Basada en tu diseño profesional:

| Color | Hex | Uso |
|-------|-----|-----|
| Azul Oscuro | `#1F4E78` | Fondo, headers, texto principal |
| Dorado | `#E7A72C` | Acentos, detalles, precios |
| Rojo Vibrante | `#D13631` | Precios finales, highlights |
| Gris Claro | `#F8F9FA` | Fondo de tarjetas |

## 🔤 Tipografías

- **Ma Shan Zheng**: Fuente caligráfica china para el título "LOOT CHINO"
- **Noto Sans SC**: Fuente moderna, limpia, para todo el contenido
- Ambas desde Google Fonts (carga rápida, sin licencias)

## 📋 Productos Incluidos

1. ✅ Mochis Sabor Fresa - $120
2. ✅ Buldak Carbonara - $50
3. ✅ Buldak Spicy Habanero - $50
4. ✅ Fideos Premium - $250
5. ✅ Té Herbal Wanglaoji - $70
6. ✅ Té Hierbas Jiduobao - $80
7. ✅ Bebida Leche de Coco - $90
8. ✅ Bebida Naranja Hong Kong - $90
9. ✅ Pocky Berries - $80
10. ✅ Galletas Naranja - $50
11. ✅ Galletas Piña - $50
12. ✅ Pocky Peach - $50
13. ✅ Polvo Matcha Premium - $150

## ✏️ Cómo Editar

### Cambiar Precios

Abre `index.html` con un editor de texto y busca:
```html
<div class="precio-value"><span class="precio-currency">$</span>120</div>
```

Reemplaza `120` por el nuevo precio.

### Cambiar Nombres o Descripciones

Busca el producto:
```html
<div class="producto-nombre">Mochi Sabor Fresa</div>
```

Y edita el texto.

### Agregar Nuevo Producto

Copia este bloque y pégalo antes de `</div>` (cierre del grid):

```html
<div class="producto-card">
    <div class="producto-imagen-container">
        <img src="imagenes/nombre-imagen.jpg" alt="Nombre Producto" class="producto-imagen">
    </div>
    <div class="producto-info">
        <div class="producto-especificaciones">
            <div class="presentacion">PESO/VOLUMEN</div>
            <div class="producto-nombre">Nombre del Producto</div>
            <div class="producto-marca">Marca</div>
        </div>
        <div class="producto-precio">
            <div class="precio-label">Precio</div>
            <div class="precio-value"><span class="precio-currency">$</span>XXX</div>
        </div>
    </div>
</div>
```

Luego actualiza:
- `nombre-imagen.jpg` → tu archivo en la carpeta `imagenes/`
- Datos del producto (peso, nombre, marca, precio)

## 🛠️ Desarrollo Local

Para ver cambios en tiempo real:

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js
npx http-server
```

Luego abre: `http://localhost:8000`

## 📱 Compatibilidad

- ✅ Chrome/Edge (Windows, Mac, Linux)
- ✅ Firefox (Windows, Mac, Linux)
- ✅ Safari (Mac, iOS)
- ✅ Tablets y móviles (iOS, Android)
- ✅ Responsive desde 320px

## 📊 Optimización

- Imágenes comprimidas (WebP, JPEG, PNG)
- CSS inline (0 requests adicionales)
- Google Fonts con display=swap (carga rápida)
- Lighthouse score: 95+

## 🔒 Privacidad y Seguridad

- ✅ Sitio estático (0 dependencias de backend)
- ✅ Sin cookies ni tracking
- ✅ Sin base de datos
- ✅ 100% HTTPS en Vercel

## 📞 Contacto

**Loot Chino** | Catálogo actualizado septiembre 2026  
☎ 2222528778

## 📄 Licencia

Todos los derechos reservados © 2026 Loot Chino

---

**Última actualización**: Septiembre 2026  
**Versión**: 1.0  
**Estado**: Producción ✅
