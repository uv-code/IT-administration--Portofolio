# 📘 IT-Administration & Cloud Portfolio

Dies ist mein persönliches IT-Portfolio, entwickelt mit **React**, **TypeScript**, **HTML**, **CSS** und **JavaScript** in **VS Code**.  
Das Projekt wird über **GitHub Actions** automatisch auf **Azure Static Web Apps** deployed.

---

## 📋 Table of Contents
- [🔍 Demo](#-demo)
- [📝 Voraussetzungen](#-voraussetzungen)
- [🏗️ Projektstruktur](#-projektstruktur)
- [⚙️ Setup](#-setup)
- [🌐 Frontend](#-frontend)
- [⚡ Deployment](#-deployment)
- [🔄 CI/CD](#-cicd)
- [📌 To Do](#-to-do)
- [👥 Mitwirken](#-mitwirken)
- [📜 License](#-license)

---

## 🔍 Demo
👉 [Live Demo](https://proud-river-080ef7d03.7.azurestaticapps.net)

---

## 📝 Voraussetzungen
- Node.js & npm installiert
- Git installiert
- GitHub Account
- Azure Static Web Apps Deployment-Token in GitHub Secrets (siehe CI/CD)

---

## 🏗️ Projektstruktur
```plaintext
project/
  public/
  src/
    App.tsx
    index.css
    main.tsx
    vite-env.d.ts
  package.json
  tsconfig.app.json
  tsconfig.json
  tsconfig.node.json
  vite.config.ts
  tailwind.config.js
.github/
  workflows/
    azure-static-web-apps-proud-river-080ef7d03.yml
README.md
```

---

## ⚙️ Setup
1. Repository klonen
   ```bash
   git clone <repository-url>
   cd dritan-portofolio/project
   ```
2. Abhängigkeiten installieren
   ```bash
   npm install
   ```
3. Dev-Server starten
   ```bash
   npm run dev
   ```
4. Öffne den Browser auf `http://localhost:5173`

---

## 🌐 Frontend
- React + TypeScript
- Vite als Build-Tool
- Tailwind CSS für Styling
- Responsive Layout

---

## ⚡ Deployment
Dieses Projekt wird mit Azure Static Web Apps deployed.

Wichtige Konfigurationen:
- App-Quellverzeichnis: `project`
- Build-Ausgabe: `dist`
- Azure Static Web Apps Workflow: `.github/workflows/azure-static-web-apps-proud-river-080ef7d03.yml`
- GitHub Secret: `AZURE_STATIC_WEB_APPS_API_TOKEN_PROUD_RIVER_080EF7D03`

Hinweis: Das Deployment wird nur für Pushes auf den Branch `main` ausgelöst.

---

## 🔄 CI/CD
Der Workflow verwendet den Azure Static Web Apps Action `Azure/static-web-apps-deploy@v1`.

Ablauf:
1. Push auf `main` oder Pull Request gegen `main`
2. Checkout des Repositories
3. Build der App im Ordner `project`
4. Upload des `dist`-Ordners zur Azure Static Web App

---

## 📌 To Do
- CI/CD-Tests hinzufügen
- Infrastruktur als Code dokumentieren
- UI weiter optimieren

---

## 👥 Mitwirken
Beiträge sind willkommen. Bitte erst ein Issue öffnen oder eine Pull Request erstellen.

---

## 📜 License
Dieses Projekt ist unter der MIT License lizenziert.










