# 🏢 Enterprise Intranet Portal with Dashboard & Analytics
 
> A modern SharePoint Online intranet serving **500+ employees daily**, built with SPFx (React + TypeScript) and embedded Power BI dashboards for real-time KPI visibility.
 
---

⚡ TL;DR
🚀 Supports 500+ daily active employees
⚡ Improved performance by ~40% (8s → 4.8s)
📈 Increased employee engagement by 65% in 60 days
📊 Integrated 5 Power BI dashboards for real-time insights
🧩 Built 8 custom SPFx web parts
🔗 Connected with Microsoft Graph API + Azure Functions

 ---
 
## 📌 Project Overview
 
| Detail | Info |
|---|---|
| **Type** | Intranet Modernization / BI & Analytics |
| **Platform** | SharePoint Online |
| **Users** | 500+ daily active employees |
| **Duration** | Enterprise-scale full lifecycle delivery |
| **Role** | SharePoint Developer (Freelance Consultant) |
 
---
 
## 🎯 Business Problem
 
The organization was running a legacy SharePoint 2013 intranet with slow page loads, no real-time data visibility, and low employee engagement. Leadership needed a modern, fast, and self-service digital workplace.
 
---
 
## ✅ Solution
 
Architected and delivered a fully modern SharePoint Online intranet with 8 custom SPFx web parts, 5 embedded Power BI dashboards, and Microsoft Graph API integration — reducing load time by ~40% and boosting engagement by ~65% within 60 days.
 
---
 
## 🛠️ Tech Stack
 
| Layer | Technologies |
|---|---|
| **Frontend** | SPFx, React, TypeScript, Fluent UI, CSS3 |
| **Backend / API** | Microsoft Graph API, Azure Functions, PnP JS |
| **Analytics** | Power BI (embedded dashboards) |
| **Platform** | SharePoint Online, Microsoft 365 |
| **Dev Tools** | VS Code, Azure DevOps, PnP PowerShell |
 
---
 
## 🧩 Custom SPFx Web Parts Built
 
| # | Web Part | Description |
|---|---|---|
| 1 | **News Feed** | Dynamic company news with filtering by department |
| 2 | **Department Hub** | Per-department landing with links, contacts & docs |
| 3 | **Quick Links** | Personalized shortcut tiles with icon support |
| 4 | **Event Calendar** | Live SharePoint calendar with month/week view |
| 5 | **KPI Tracker** | Live metric cards pulling from Power BI datasets |
| 6 | **Org Directory** | Graph API-powered searchable employee directory |
| 7 | **Weather Widget** | Location-aware weather using external API |
| 8 | **Announcements** | Priority-based alert banner with dismissal |
 
---
 
## 📊 Power BI Dashboards Embedded
 
- Finance — Budget vs Actuals, spend trends
- HR — Headcount, attrition, leave analytics
- IT — Ticket volume, SLA compliance, asset status
- Operations — Project status, delivery KPIs
- Sales — Pipeline, revenue targets, regional performance
 
---
 
## 📈 Results & Impact
 
| Metric | Before | After |
|---|---|---|
| Page load time | ~8 seconds (SP 2013) | ~4.8 seconds (~40% faster) |
| Employee engagement | Baseline | **+65% within 60 days** |
| Self-service adoption | Manual email requests | Full self-service portal |
| BI reporting | Manual Excel reports | Live embedded dashboards |
 
---
 
## 🏗️ Architecture Overview
 
```
SharePoint Online
│
├── SPFx Web Parts (React + TypeScript + Fluent UI)
│   ├── News Feed
│   ├── KPI Tracker ──────────── Power BI Embedded
│   ├── Org Directory ─────────── Microsoft Graph API
│   └── Event Calendar ────────── SharePoint List
│
├── Azure Functions (serverless backend)
│   └── External API calls (Weather, 3rd-party KPIs)
│
└── PnP JS / REST API
    └── SharePoint List & Library operations
```
 
---
 
## 🔐 Governance & Security
 
- RBAC enforced across all site collections
- Audience targeting on web parts per department
- Content approval workflows for news publishing
- Compliance-aligned retention policies on libraries
 
---
 
## 📁 Repository Structure
 
```
📦 sharepoint-intranet-portal
 ┣ 📂 src
 ┃ ┣ 📂 webparts
 ┃ ┃ ┣ 📂 newsFeed
 ┃ ┃ ┣ 📂 departmentHub
 ┃ ┃ ┣ 📂 quickLinks
 ┃ ┃ ┣ 📂 eventCalendar
 ┃ ┃ ┣ 📂 kpiTracker
 ┃ ┃ ┣ 📂 orgDirectory
 ┃ ┃ ┣ 📂 weatherWidget
 ┃ ┃ └ 📂 announcements
 ┃ ┣ 📂 extensions
 ┃ └ 📂 shared
 ┃   ┣ 📂 components
 ┃   ┣ 📂 services
 ┃   └ 📂 utils
 ┣ 📂 config
 ┣ 📂 docs
 ┃ ┣ 📄 architecture.md
 ┃ ┣ 📄 deployment-guide.md
 ┃ └ 📄 web-part-catalog.md
 ┣ 📄 package.json
 ┣ 📄 tsconfig.json
 └ 📄 README.md
```
 
---
 
## 🚀 Deployment
 
1. Clone the repo
2. Run `npm install`
3. Update `config/serve.json` with your SharePoint site URL
4. Run `gulp serve` for local development
5. Run `gulp bundle --ship && gulp package-solution --ship` for production
6. Upload `.sppkg` to SharePoint App Catalog
7. Deploy to site collection
 
---
 
## 📬 Contact
 
**Bobba S Jaswanth Chowdary** — SharePoint Developer  
📧 bobbajasswanthchowdary@gmail.com  
🔗 [linkedin.com/in/jaswanthchowdarybobba](https://www.linkedin.com/in/jaswanthchowdarybobba/)
