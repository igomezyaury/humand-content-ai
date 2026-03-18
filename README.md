# 🚀 Humand Content AI

Generador inteligente de calendario de contenidos para el **Muro de Humand.co** — con copy listo para publicar e imágenes con identidad corporativa, todo en minutos.

---

## ✨ ¿Qué hace?

| Feature | Descripción |
|---|---|
| 🎨 **Extracción de marca** | Analiza el sitio web de tu empresa y extrae colores, tipografía y estilo automáticamente |
| 🗓 **Calendario mensual** | Genera un calendario visual con publicaciones distribuidas inteligentemente en días laborables |
| 📝 **3 versiones de copy** | Principal (con emojis + CTA), Corto/urgente y Formal/ejecutivo por cada post |
| 🖼 **Imágenes con identidad** | Genera imágenes en 3 formatos (1:1, 4:5, 16:9) con los colores reales de la empresa |
| 🏢/🎨 **Estilos de imagen** | Elige entre Realista/Corporativo o Ilustración/Flat Design por post |
| ⬇ **Exportación** | Descarga imágenes en SVG (vectorial) y PNG, exporta el calendario en TXT |
| 🔄 **Regeneración** | Regenera cualquier post o imagen individual si no convence |

---

## 🏃 Cómo usar

### Opción 1 — Abrir directo en el navegador
Descarga `index.html` y ábrelo en tu navegador. No requiere servidor ni instalación.

### Opción 2 — GitHub Pages (recomendado)
1. Haz fork de este repositorio
2. Ve a **Settings → Pages**
3. Selecciona `main` branch como fuente
4. Tu app estará disponible en `https://tu-usuario.github.io/humand-content-ai`

### Opción 3 — Servidor local
```bash
git clone https://github.com/tu-usuario/humand-content-ai.git
cd humand-content-ai
# Con Python:
python3 -m http.server 8080
# Con Node.js:
npx serve .
```
Abre `http://localhost:8080`

---

## 🔧 Flujo de trabajo recomendado

```
1. Ingresa el sitio web de la empresa → "Analizar"
   ↓ La IA extrae colores, tipografía y estilo

2. Configura mes, tono(s), frecuencia y categorías
   ↓

3. "Generar calendario completo"
   ↓ Calendario + sugerencias estratégicas + copy de cada post

4. Por cada post: "🎨 Imagen" → elige estilo → genera 3 formatos
   O: "🎨 Generar todas las imágenes" para procesar el mes entero

5. Copia el copy directo al Muro de Humand
   Descarga la imagen en PNG o SVG
```

---

## ⚙️ Configuración

La app usa la **API de Anthropic (Claude)** directamente desde el navegador. El endpoint está incluido en el HTML — funciona sin configuración adicional cuando se usa desde claude.ai o con una API key válida.

Para uso independiente (fuera de claude.ai), agrega tu API key en el header de las llamadas fetch:
```javascript
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'TU_API_KEY',
  'anthropic-version': '2023-06-01'
}
```

---

## 📁 Estructura del proyecto

```
humand-content-ai/
├── index.html          # App completa (single file)
├── README.md           # Este archivo
├── .github/
│   └── workflows/
│       └── deploy.yml  # Auto-deploy a GitHub Pages
└── docs/
    └── screenshot.png  # Preview de la app
```

---

## 🎯 Categorías de contenido soportadas

- 📢 **Comunicado** — Anuncios oficiales, cambios organizacionales
- 🏆 **Reconocimiento** — Logros de equipos y colaboradores
- 💚 **Bienestar** — Salud mental, equilibrio trabajo-vida
- 🎯 **Cultura** — Valores, tradiciones, identidad corporativa
- 📚 **Capacitación** — Aprendizaje, desarrollo profesional
- 📰 **Noticias** — Actualizaciones del sector, logros de la empresa

---

## 🤝 Casos de uso

- **Equipos de RRHH** — Planificación mensual del Muro de Humand sin depender de diseñadores
- **Comunicación interna** — Contenido consistente con la identidad de marca
- **Marketing de employer branding** — Calendario estratégico alineado con fechas clave

---

## 📄 Licencia

MIT — Libre para uso comercial y personal.

---

*Construido con ❤️ usando Claude (Anthropic) · Diseñado para equipos que usan Humand.co*
