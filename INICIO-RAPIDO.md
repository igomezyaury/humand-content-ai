# 🚀 Humand Content AI — Inicio Rápido

## ¿Qué es este proyecto?
Herramienta de IA para generar calendarios de contenido mensual para el Muro de Humand.co.
Genera copy en 3 versiones, imágenes con identidad de marca y exporta a PowerPoint, Gamma o Canva.

---

## Opción 1 — Abrirlo directo (sin instalar nada)
1. Abre el archivo `index.html` en Chrome, Safari o Edge
2. ¡Listo! La app funciona directo en el navegador

---

## Opción 2 — Subirlo a internet gratis con Netlify
1. Ve a **netlify.com/drop**
2. Arrastra el archivo `index.html` a la página
3. Haz clic en **"Rename and deploy"**
4. Obtienes un link tipo `https://nombre.netlify.app` para compartir con todo el equipo

---

## Opción 3 — Subir a GitHub Pages (para el equipo de tech)
1. Crea un repositorio nuevo en github.com
2. Sube todos los archivos de esta carpeta
3. Ve a Settings → Pages → selecciona branch `main`
4. Tu app queda en `https://tu-usuario.github.io/humand-content-ai`
El archivo `.github/workflows/deploy.yml` hace el deploy automático en cada cambio.

---

## Cómo usar la app
1. **Ingresa el sitio web** de la empresa → clic en "Analizar" para extraer colores automáticamente
2. **Configura** nombre, industria, tono(s), mes y categorías
3. Clic en **"Generar calendario completo"** — la IA crea todo el mes
4. Por cada publicación: copia el texto o genera la imagen con identidad de marca
5. Usa **"📤 Exportar"** para llevar todo a PowerPoint, Gamma o Canva

---

## Estructura del proyecto
```
index.html          ← App completa (todo en un solo archivo)
README.md           ← Documentación técnica
INICIO-RAPIDO.md    ← Esta guía
.github/
  workflows/
    deploy.yml      ← Auto-deploy a GitHub Pages
```

---

## ¿Problemas o mejoras?
Vuelve a la conversación de Claude y pide los cambios — se genera un nuevo `index.html` actualizado.
