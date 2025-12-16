# Tablao Flamenco Las Setas — Web Assets

Repositorio de **código personalizado** para la web de Tablao Flamenco Las Setas (WordPress + Elementor Pro).

> **Desarrollador:** @clicandwords  
> **Estado:** En desarrollo (entorno test)  
> **Versión actual:** v3.0

---

## 📁 Estructura

```
tablao-las-setas-web/
├── css/
│   └── tablao-las-setas-css-v3.css    # CSS global (2244 líneas)
├── js/
│   ├── footer-scripts.html             # Turitop + UX (smooth scroll, sticky CTA)
│   └── tracking.html                    # gtag + fbq (separado para GDPR)
├── schema/
│   └── head-schema.html                 # Schema markup SEO/IA
├── sections/                            # HTML reutilizable (próximamente)
└── README.md
```

---

## 🎨 Diseño

### Colores
| Nombre | Hex | Uso |
|--------|-----|-----|
| Rojo Pantone 200C | `#C8102E` | Fondo principal, CTAs |
| Negro cálido | `#1A1512` | Textos, footer |
| Oro harvest | `#E3AD43` | Acentos, botones hover |
| Crema | `#F9E5DA` | Texto sobre fondos oscuros |

### Tipografías
| Uso | Fuente |
|-----|--------|
| H1 Hero | Geoparody |
| H2, H3 | Bright Almond |
| Body | Work Sans |
| Botones | Montserrat |

### Clases CSS principales
| Elemento | Clase |
|----------|-------|
| Header | `.tfs-header-main` |
| Top bar | `.tfs-top-bar` |
| Botón CTA | `.tfs-btn-primary` |
| Cards artistas | `.tfs-artist-card` |

---

## 📄 Páginas (15)

### Menú principal
| Página | Slug | Notas |
|--------|------|-------|
| Home | `/` | Hero + Turitop + Secciones |
| Espectáculo Flamenco | `/espectaculo-flamenco-sevilla/` | Página padre |
| → Elenco | `/elenco/` | Grid artistas + modal |
| → Nosotros | `/nosotros/` | Historia + Sandra Guerrero |
| Entradas y Horarios | `/entradas-horarios/` | Widget Turitop |
| Ubicación | `/ubicacion/` | Mapa + instrucciones |
| Programación | `/programacion/` | MEC shortcode 3057 |
| Carta | `/carta/` | Cócteles + vinos + tapas |
| Contacto | `/contacto/` | Formulario + WhatsApp |
| FAQs | `/faqs/` | Preguntas frecuentes |
| Blog | `/blog/` | Archivo + posts |

### Legales (footer)
Aviso Legal · Política Privacidad · Política Cookies · Condiciones Cancelación · Condiciones Uso Web

---

## ⚡ Implementación rápida

### 1. CSS global
```
WordPress → Apariencia → Personalizar → CSS adicional
Pegar: css/tablao-las-setas-css-v3.css
```

### 2. Schema (en HEAD)
```
WPCode → Header & Footer → Header
Pegar: schema/head-schema.html
```

### 3. Scripts (en FOOTER)
```
WPCode → Header & Footer → Footer
Pegar: js/footer-scripts.html

⚠️ Si usas banner de cookies/consent:
Pegar tracking.html SOLO cuando haya consentimiento
(o integrarlo con tu CMP)
```

---

## 📦 Detalle de archivos

### CSS (`css/tablao-las-setas-css-v3.css`)
- Variables `:root`
- Header / Top bar / Footer
- Formularios
- TranslatePress
- Blog
- Responsive
- Secciones Home

### Schema (`schema/head-schema.html`)
| Schema | Contenido |
|--------|-----------|
| LocalBusiness | Datos negocio, coordenadas, horarios |
| EventSeries | 3 pases diarios con precios |
| FAQPage | 15 preguntas optimizadas para IA |

**Datos incluidos (verificar periódicamente):**
| Dato | Valor | Fuente | Última verificación |
|------|-------|--------|---------------------|
| Rating | 4.9/5 | Google + GYG | Dic 2024 |
| Reviews | ~13,000 | Google 11K + GYG 2K | Dic 2024 |

### Scripts (`js/footer-scripts.html`)
- Turitop (empresa T1263, color #E3AD43)
- Smooth scroll
- Sticky CTA (IntersectionObserver)

### Tracking (`js/tracking.html`) ⚠️
- Google Analytics (gtag)
- Facebook Pixel (fbq)

> **GDPR:** Este archivo debe cargarse SOLO con consentimiento del usuario.
> Integrarlo con tu CMP (Complianz, CookieYes, etc.)

---

## 🔌 Plugins

| Plugin | Uso | Config |
|--------|-----|--------|
| Elementor Pro | Page builder | - |
| MEC | Programación | Shortcode 3057, skin acordeón |
| Turitop | Reservas | Empresa T1263 |
| TranslatePress | Multiidioma | ES, EN |
| Trustindex | Reviews | Widget embebido |
| Click to Chat | WhatsApp | +34 684 776 981 |
| WPCode | Headers/Footers | Schema + Scripts |

---

## 🔄 Variables y Replace

Antes de pasar a **producción**, buscar y reemplazar:

| Buscar | Reemplazar por |
|--------|----------------|
| `test.tablaoflamencolassetas.com` | `tablaoflamencolassetas.com` |

**Revisar también:**
- [ ] ID shortcode MEC (actualmente 3057)
- [ ] ID empresa Turitop (actualmente T1263)
- [ ] IDs de analytics/píxeles si cambian

---

## ✅ Checklist de publicación

```
□ Replace test → prod (dominio, embeds)
□ Schema: Rich Results Test sin errores
□ Lighthouse móvil: LCP < 2.5s, CLS < 0.1
□ Imágenes: WebP + lazy-load
□ Tracking: eventos OK + consent configurado
□ Responsive: 375px / 768px / 1024px / 1440px
□ Formularios: labels + validación
```

---

## 📞 Datos del negocio

| Campo | Valor |
|-------|-------|
| **Nombre** | Tablao Flamenco Las Setas |
| **Dirección** | Plaza de la Encarnación 38, 41003 Sevilla |
| **Tel/WhatsApp** | +34 684 776 981 |
| **Email** | reservas@tablaoflamencolassetas.com |
| **Shows** | 18:00 · 19:45 · 21:30 (+16:30 y 23:15 temporada alta) |
| **Duración** | 75 min (descanso 5-10 min) |
| **Aforo** | 140 plazas |
| **Directora** | Sandra Guerrero "La Negra" |

### Precios
| Tipo | € | Incluye |
|------|---|---------|
| Básica | 28 | Solo show, laterales |
| General | 38 | Show + cóctel, laterales preferentes |
| Premium | 50 | Show + bebida + tapa, vista frontal |
| VIP | 68 | Show + 2 bebidas + 2 tapas, 1ª fila |

---

## 📝 Changelog

### v3.0
- ✅ CSS organizado (2244 líneas, código muerto eliminado)
- ✅ Schema completo (LocalBusiness, EventSeries, FAQPage)
- ✅ Footer scripts (Turitop + UX)
- ✅ Tracking separado (GDPR)

### Próximos pasos
- [ ] Ajustar layout MEC acordeón
- [ ] Añadir idiomas DE/FR
- [ ] Optimizar imágenes WebP
- [ ] Crear `/sections` con módulos HTML

---

## 🔗 Enlaces

- [Google Rich Results Test](https://search.google.com/test/rich-results)
- [Schema Validator](https://validator.schema.org/)
- [PageSpeed Insights](https://pagespeed.web.dev/)

---

*Repositorio mantenido por @clicandwords*
