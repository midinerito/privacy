# Mi Dinerito — Política de privacidad pública

Sitio web estático que aloja la política de privacidad oficial de **Mi Dinerito**, la aplicación
Android educativa de finanzas para niños de 5 a 12 años.

🌐 **URL pública (producción):** https://midinerito.github.io/privacy/

- 🇪🇸 Español: [`/`](https://midinerito.github.io/privacy/)
- 🇬🇧 English: [`/en.html`](https://midinerito.github.io/privacy/en.html)

---

## Por qué este repositorio

Google Play Console exige una URL **pública, accesible y sin geofencing** para la política de
privacidad. La aplicación principal de Mi Dinerito vive en un repositorio privado (código
propietario); este repo separado contiene únicamente el documento legal en HTML, expuesto vía
GitHub Pages.

## Estructura

```
.
├── index.html    Política en español (versión por defecto).
├── en.html       Política en inglés.
├── style.css     Estilos compartidos (paleta y patrones del design system de la app).
├── README.md     Este archivo.
└── LICENSE       Licencia del repositorio (CC BY-ND 4.0).
```

## Previsualización local

Es HTML estático. Para verlo localmente:

```bash
# Opción 1: abrir directamente en el navegador
xdg-open index.html        # Linux
open index.html            # macOS
start index.html           # Windows

# Opción 2: servidor local (para probar paths relativos)
python3 -m http.server 8000
# luego abrir http://localhost:8000
```

## Características técnicas

- ✅ Sin JavaScript — cero superficie de tracking accidental.
- ✅ Sin fuentes externas (Google Fonts, etc.) — stack del sistema, máxima privacidad y rendimiento.
- ✅ Sin imágenes pesadas — emojis con `fontFamilyFallback` y SVG inline si hace falta.
- ✅ Mobile-first responsive (Play Store la abre primero desde móvil).
- ✅ Dark mode automático (`prefers-color-scheme`).
- ✅ Accesibilidad: skip-link, contraste AA, semantic HTML, `aria-label`, `aria-current`.
- ✅ SEO multi-idioma: `hreflang` correctos, `canonical` por versión, `x-default`.

## Estilos

La paleta y patrones (NeoCard, pill chips de sección, tipografía bold) reproducen el design system
de la app Android (`docs/design/DESIGN_SYSTEM.md` del repo principal) para coherencia visual entre
ambos productos.

## Histórico de cambios

Los commits de este repositorio actúan como historial público de cambios de la política. Cada
actualización significativa actualiza también el campo "Última actualización" / "Last updated" en
el pie de las páginas.

## Contacto legal

Para ejercicio de derechos RGPD o cualquier consulta:

**Angel Miguel Friero Calvo**
📧 angel.friero@proton.me

---

> ⚖️ El contenido de la política refleja las prácticas reales de tratamiento de datos de Mi Dinerito
> y sigue las directrices de la AEPD y de Google Play Families Policy. No constituye asesoramiento
> legal para terceros.
