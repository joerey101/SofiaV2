# Sofia Github — Documentación del Proyecto

## ¿Qué es este proyecto?

Este es el sitio web oficial de **Sofía Destefano**, coach ontológica especializada en transformación personal y organizacional. El código fuente original fue desarrollado por el equipo de Sofia y vive en este repositorio.

---

## Repositorio y Conexiones

| Elemento | Valor |
|---|---|
| **Repositorio original** | `https://github.com/sofiadestefano-eng/sofia.git` |
| **Repositorio de trabajo (José)** | `https://github.com/joerey101/SofiaV2.git` |
| **Carpeta local** | `/Users/joserey/Documents/@Trabajo/Proyectos IA/Sofi Github/` |
| **Puerto de desarrollo** | `http://localhost:5173` |

---

## Stack Tecnológico

- **Framework:** React 18 + Vite
- **Lenguaje:** JavaScript (`.jsx`)
- **Estilos:** Tailwind CSS
- **Routing:** React Router DOM
- **Animaciones:** Framer Motion
- **Íconos:** lucide-react `v0.474.0` ⚠️ (ver nota abajo)
- **Formularios:** React Hook Form

> ⚠️ **Nota sobre lucide-react:** Se mantiene en la versión `0.474.0` intencionalmente. Las versiones `1.x` eliminaron los íconos de redes sociales (`Instagram`, `Linkedin`) que usa el `Footer.jsx`. **No actualizar** sin revisar primero.

---

## Estructura del Proyecto

```
Sofi Github/
├── public/
│   ├── favicon.svg
│   └── icons.svg
├── src/
│   ├── assets/          ← Imágenes (hero.jpg, hero.png)
│   ├── components/
│   │   ├── Footer.jsx   ← Footer con redes sociales
│   │   └── Navbar.jsx   ← Navegación principal
│   ├── data/
│   │   └── siteData.js  ← TODO EL CONTENIDO CENTRALIZADO ACÁ
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── SobreSofia.jsx
│   │   ├── Servicios.jsx
│   │   ├── Resultados.jsx
│   │   └── Contacto.jsx
│   ├── styles/
│   │   └── globals.css
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── package.json
├── tailwind.config.js
├── vite.config.js
└── index.html
```

---

## Contenido Centralizado (`src/data/siteData.js`)

**Todo el texto del sitio vive en este archivo.** Para actualizar contenido (textos, testimonios, redes sociales, email) editá solo este archivo sin tocar los componentes.

Incluye:
- Nombre y tagline de Sofía
- Descripción de servicios (Coaching Organizacional y Personal)
- Lista de ítems por servicio
- Testimonios (4 testimonios de clientes)
- Navegación del sitio
- URLs de redes sociales (Instagram, LinkedIn, WhatsApp)
- Email de contacto

---

## Páginas del Sitio

| Ruta | Página |
|---|---|
| `/` | Home |
| `/sobre-sofia` | Sobre Sofía |
| `/servicios` | Servicios |
| `/resultados` | Resultados y testimonios |
| `/contacto` | Formulario de contacto |

---

## Cómo levantar el proyecto localmente

```bash
# 1. Entrar a la carpeta
cd "/Users/joserey/Documents/@Trabajo/Proyectos IA/Sofi Github"

# 2. Instalar dependencias
npm install

# 3. Iniciar servidor de desarrollo
npm run dev
# → http://localhost:5173
```

---

## Cómo deployar a Vercel

Este proyecto está conectado al repositorio `https://github.com/joerey101/SofiaV2.git`.

**Cualquier `git push` a `main` dispara un deploy automático en Vercel.**

Para deploy manual desde la terminal:
```bash
git add .
git commit -m "descripción del cambio"
git push origin main
```

### Configuración de Vercel
- **Framework:** Vite (detección automática)
- **Build command:** `npm run build`
- **Output directory:** `dist`

---

## TODOs Pendientes

- [ ] Reemplazar URLs de redes sociales por las reales en `siteData.js` (`instagram`, `linkedin`, `whatsapp`)
- [ ] Actualizar el email de contacto en `siteData.js`
- [ ] Reemplazar las imágenes de `src/assets/` con las fotos reales de Sofía
- [ ] Configurar formulario de contacto con servicio de email real (Resend, EmailJS, etc.)
- [ ] Revisar y ajustar el copy de cada sección con Sofía

---

## Proyecto Relacionado

Existe un segundo proyecto más avanzado con diseño mejorado (TypeScript + Tailwind + animaciones + shadcn):
- **Repositorio:** `https://github.com/joerey101/Sofi.git`
- **Carpeta local:** `/Users/joserey/Documents/@Trabajo/Proyectos IA/sofi/sofia-coaching/`
