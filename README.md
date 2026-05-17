# ✂️ ClipForge — AI Clip Generator

Generador de clips virales powered by Claude AI. Sin límites, sin créditos.

---

## ⚠️ Por qué necesitás un servidor local

Los navegadores bloquean las llamadas directas a `api.anthropic.com` por política de seguridad **CORS**.
La solución es este servidor Node.js que actúa de **proxy**: el browser le pega al servidor local,
y el servidor le pega a Anthropic con tu API key desde el backend.

```
Browser → localhost:3000/api/analyze → api.anthropic.com
```

---

## 🚀 Instalación y uso

### 1. Instalá las dependencias (solo la primera vez)

```bash
npm install
```

### 2. Configurá tu API key

Editá el archivo `.env` y pegá tu API key de Anthropic:

```
ANTHROPIC_API_KEY=sk-ant-tu-clave-aqui
```

> Conseguí tu API key en: https://console.anthropic.com/

### 3. Iniciá el servidor

```bash
node server.js
```

### 4. Abrí el navegador

```
http://localhost:3000
```

---

## 📁 Estructura del proyecto

```
clipforge/
├── server.js        ← Servidor proxy (Node.js + Express)
├── .env             ← Tu API key (no compartir)
├── package.json
└── public/
    └── index.html   ← Frontend completo
```

---

## 🔑 Cómo obtener tu API key

1. Entrá a https://console.anthropic.com/
2. Andá a **API Keys** → **Create Key**
3. Copiá la clave y pegala en el `.env`

---

## ∞ Sin límites

A diferencia de Opus Clip, esta app no tiene sistema de créditos.
Usás tu propia API key de Anthropic y pagás solo por lo que consumís
(los precios de Claude Sonnet son muy accesibles).
