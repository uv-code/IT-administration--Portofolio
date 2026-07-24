# Dritan Shehaj – IT Portfolio

Responsives IT-Administrator-Portfolio mit React, Vite und Tailwind CSS.

## Lokale Entwicklung

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

Der Build-Output liegt im Ordner `dist/`.

## Deployment auf Azure Static Web Apps

### Variante 1 — Über GitHub (empfohlen)

1. Repository auf GitHub pushen (inklusive `.github/workflows/azure-static-web-apps.yml`).
2. Im [Azure Portal](https://portal.azure.com) eine neue **Static Web App** erstellen.
3. Als Bereitstellungsquelle **GitHub** wählen und das Repository verknüpfen.
4. Azure legt automatisch das Secret `AZURE_STATIC_WEB_APPS_API_TOKEN` an und startet den ersten Deployment-Lauf.
5. Nach erfolgreichem Build ist die Seite unter der Azure-URL erreichbar.

Build-Einstellungen im Azure Wizard:
- **Framework:** React
- **Build command:** `npm run build`
- **Output location:** `dist`

### Variante 2 — Azure CLI (SWA CLI)

```bash
npm install -g @azure/static-web-apps-cli
npm run build
swa deploy dist
```

## Struktur

```
├── .github/workflows/   GitHub Actions Workflow für Azure
├── public/              Statische Dateien + SPA-Routing-Konfig
├── src/                 React-Quellcode
│   └── App.tsx          Hauptkomponente mit allen Sektionen
├── index.html           HTML-Einstiegspunkt
└── tailwind.config.js   Tailwind-Theme
```
