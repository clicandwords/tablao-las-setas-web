# tablao-las-setas-web
Código CSS y HTML para la web del Tablao Flamenco Las Setas


# Tablao Flamenco Las Setas - Web Assets

Repositorio de código personalizado para la web **tablaoflamencolassetas.com** (WordPress + Elementor Pro).

> **Última actualización:** Diciembre 2024  
> **Desarrollador:** @clicandwords  
> **Estado:** En desarrollo (entorno test)

---

## 📁 Estructura del repositorio

```
tablao-las-setas-web/
├── css/
│   └── tablao-las-setas-css-v3.css    # CSS global (2244 líneas)
├── js/
│   └── footer-scripts.html             # Turitop + JS personalizado
├── schema/
│   └── head-schema.html                # Schema markup SEO/IA
├── sections/                            # Secciones HTML reutilizables
│   └── (próximamente)
└── README.md
```

---

## 🎨 Paleta de colores

| Nombre | Hex | Uso |
|--------|-----|-----|
| Rojo Pantone 200C | `#C8102E` | Fondo principal, CTAs |
| Negro cálido | `#1A1512` | Textos, footer |
| Oro harvest | `#E3AD43` | Acentos, botones hover |
| Crema cálido | `#F9E5DA` | Texto sobre fondos oscuros |
| Off-white | `#FCE2BF` | Texto principal |

---

## 🔤 Tipografías

| Uso | Fuente |
|-----|--------|
| H1 Hero | Geoparody |
| H2, H3 | Bright Almond |
| Subtítulos especiales | Fifties Movies |
| Decorativo | Flowers Kingdom |
| Body text | Work Sans / Lato |
| Botones | Montserrat |

---

## 📄 Páginas de la web (15)

### Menú principal

| # | Página | Slug | Estado | Notas |
|---|--------|------|--------|-------|
| 1 | **Home** | `/` | ✅ Activa | Hero + Turitop + Secciones |
| 2 | **Espectáculo Flamenco** | `/espectaculo-flamenco-sevilla/` | ✅ Activa | Página padre con desplegable |
| 2a | → Elenco | `/elenco/` | ✅ Activa | Grid artistas + modal popup |
| 2b | → Nosotros | `/nosotros/` | ✅ Activa | Historia + Sandra Guerrero |
| 3 | **Entradas y Horarios** | `/entradas-horarios/` | ✅ Activa | Widget Turitop embebido |
| 4 | **Ubicación** | `/ubicacion/` | ✅ Activa | Mapa + instrucciones |
| 5 | **Programación** | `/programacion/` | ✅ Activa | MEC shortcode 3057 (acordeón) |
| 6 | **Carta** | `/carta/` | ✅ Activa | Cócteles + vinos Jerez + tapas |
| 7 | **Contacto** | `/contacto/` | ✅ Activa | Formulario + WhatsApp |
| 8 | **FAQs** | `/faqs/` | ✅ Activa | Preguntas frecuentes |
| 9 | **Blog** | `/blog/` | ✅ Activa | Archivo + 1 post |

### Páginas legales (footer)

| # | Página | Slug | Estado |
|---|--------|------|--------|
| 10 | Aviso Legal | `/aviso-legal/` | ✅ |
| 11 | Política Privacidad | `/politica-privacidad/` | ✅ |
| 12 | Política Cookies | `/politica-cookies/` | ✅ |
| 13 | Condiciones Cancelación | `/condiciones-cancelacion/` | ✅ |
| 14 | Condiciones Uso Web | `/condiciones-uso-web/` | ✅ |

---

## 📦 Archivos del repositorio

### 1. CSS Global (`/css/tablao-las-setas-css-v3.css`)

**Líneas:** ~2244  
**Implementación:** Pegarlo en **Apariencia → Personalizar → CSS adicional** o plugin WPCode

**Secciones incluidas:**
- Variables CSS (`:root`)
- Header sticky (`tfs-header-main`, `tfs-top-bar`)
- Footer completo
- Formularios
- TranslatePress estilos
- Blog y posts
- Responsive breakpoints
- Home 2025 secciones

### 2. Schema Markup (`/schema/head-schema.html`)

**Implementación:** Plugin **Insert Headers and Footers (WPCode)** → Sección Header

**Contenido:**
- `LocalBusiness` + `TouristAttraction` + `PerformingArtsTheater`
- `EventSeries` con 3 subEvents (18:00, 19:45, 21:30)
- `FAQPage` con 15 preguntas optimizadas para IA
- Preconnects y preloads optimizados

**Datos clave:**
| Campo | Valor |
|-------|-------|
| Rating | 4.9/5 |
| Reviews | 13,000 (Google 11K + GetYourGuide 2K) |
| Precios | 28€ - 68€ (4 tipos entrada) |
| Duración | 75 minutos |
| Artistas | 8 profesionales |

### 3. Footer Scripts (`/js/footer-scripts.html`)

**Implementación:** Plugin **WPCode** → Sección Footer

**Contenido:**
- Script Turitop (empresa T1263, color #E3AD43)
- Smooth scroll para enlaces internos
- Sticky CTA con IntersectionObserver
- Event tracking (gtag + fbq)

---

## 🔌 Plugins requeridos

| Plugin | Uso | Config clave |
|--------|-----|--------------|
| **Elementor Pro** | Page builder | - |
| **Modern Events Calendar (MEC)** | Programación | Shortcode 3057, skin acordeón |
| **Turitop** | Reservas | Empresa T1263 |
| **TranslatePress** | Multiidioma | ES, EN, (DE, FR próx.) |
| **Trustindex** | Reviews Google | Widget embebido |
| **Click to Chat** | WhatsApp | +34 684 776 981 |
| **WPCode** | Headers/Footers | Schema + Scripts |

---

## 📋 Implementación paso a paso

### CSS Global
1. Ir a **Apariencia → Personalizar → CSS adicional**
2. Pegar contenido de `/css/tablao-las-setas-css-v3.css`
3. Publicar

### Schema Markup
1. Instalar plugin **WPCode** (Insert Headers and Footers)
2. Ir a **Code Snippets → Header & Footer**
3. En sección **Header**, pegar contenido de `/schema/head-schema.html`
4. Guardar

### Footer Scripts
1. En mismo plugin WPCode
2. En sección **Footer**, pegar contenido de `/js/footer-scripts.html`
3. Guardar

### Validación
1. Abrir [Google Rich Results Test](https://search.google.com/test/rich-results)
2. Introducir URL de la web
3. Verificar que detecta LocalBusiness, Event y FAQ

---

## ⚠️ Notas importantes

### URLs de desarrollo
Todos los archivos usan `test.tablaoflamencolassetas.com`. 

**Antes de pasar a producción:**
- Buscar y reemplazar `test.tablaoflamencolassetas.com` → `tablaoflamencolassetas.com`

### Clases CSS principales
| Elemento | Clase |
|----------|-------|
| Header principal | `.tfs-header-main` |
| Top bar | `.tfs-top-bar` |
| Contenedor hero | `.tfs-hero` |
| Cards artistas | `.tfs-artist-card` |
| Botón CTA | `.tfs-btn-primary` |

### MEC (Calendario)
- **Shortcode activo:** `[MEC id="3057"]`
- **Skin:** Acordeón
- **Campos personalizados:** Baile, Cante, Guitarra, Percusión
- **Pendiente:** Ajustar layout del acordeón desplegado

---

## 📞 Datos del negocio

| Campo | Valor |
|-------|-------|
| **Nombre** | Tablao Flamenco Las Setas |
| **Dirección** | Plaza de la Encarnación 38, 41003 Sevilla |
| **Teléfono/WhatsApp** | +34 684 776 981 |
| **Email** | reservas@tablaoflamencolassetas.com |
| **Horarios shows** | 18:00 · 19:45 · 21:30 (+ 16:30 y 23:15 en temporada alta) |
| **Duración** | 75 minutos (con descanso 5-10 min) |
| **Aforo** | 140 plazas |
| **Directora artística** | Sandra Guerrero "La Negra" |

### Precios entradas
| Tipo | Precio | Incluye |
|------|--------|---------|
| Básica | 28€ | Solo show, asientos laterales |
| General | 38€ | Show + cóctel/bebida, laterales preferentes |
| Premium | 50€ | Show + bebida + tapa gourmet, vista frontal |
| VIP | 68€ | Show + 2 bebidas + 2 tapas, primera fila |

---

## 📝 Changelog

### v3.0 (Diciembre 2024)
- ✅ CSS limpio y organizado (eliminado código muerto)
- ✅ Schema markup completo (LocalBusiness, EventSeries, FAQPage)
- ✅ Footer scripts con Turitop y tracking
- ✅ Datos verificados (precios, reviews, servicios)

### Próximos pasos
- [ ] Ajustar layout MEC acordeón desplegado
- [ ] Añadir más idiomas (DE, FR)
- [ ] Optimizar imágenes WebP
- [ ] Crear secciones HTML reutilizables

---

## 🔗 Enlaces útiles

- **Web test:** https://test.tablaoflamencolassetas.com
- **Web producción:** https://tablaoflamencolassetas.com
- **Google Rich Results Test:** https://search.google.com/test/rich-results
- **Schema Validator:** https://validator.schema.org/

---

*Repositorio mantenido por @clicandwords para Tablao Flamenco Las Setas*
