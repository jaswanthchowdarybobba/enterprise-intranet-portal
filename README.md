# 🏢 Enterprise Intranet Portal (SharePoint + SPFx + Power BI)

> A modern, high-performance SharePoint Online intranet serving **500+ daily users**, featuring real-time analytics dashboards, personalized experiences, and enterprise-grade architecture.

---

## ⚡ TL;DR

* 🚀 Supports **500+ daily active employees**
* ⚡ Improved performance by **~40% (8s → 4.8s)**
* 📈 Increased employee engagement by **65% in 60 days**
* 📊 Integrated **5 Power BI dashboards** for real-time insights
* 🧩 Built **8 custom SPFx web parts**
* 🔗 Connected with **Microsoft Graph API + Azure Functions**

 ---
 

<!-- ============================================================ -->
<!--  TWO COLUMN LAYOUT — like SharePoint Section with 2 columns  -->
<!-- ============================================================ -->

<table width="100%" cellspacing="0" cellpadding="0">
<tr valign="top">

<!-- LEFT COLUMN -->
<td width="65%" style="padding-right:16px;">

### 📋 About This Project

> A fully modern SharePoint Online intranet built to replace a legacy SharePoint 2013 environment. Architected with 8 custom SPFx web parts (React + TypeScript + Fluent UI), 5 embedded Power BI dashboards, and Microsoft Graph API integration for live org data — reducing page load time by ~40% and boosting employee engagement by ~65% within 60 days of launch.

---

### 🧩 Custom SPFx Web Parts

| Web Part | Description | Tech |
|---|---|---|
| 📰 **News Feed** | Dynamic company news with department filtering | SPFx + REST API |
| 🏛 **Department Hub** | Per-department landing with links and contacts | SPFx + Graph API |
| 🔗 **Quick Links** | Personalized shortcut tiles with icon support | SPFx + SharePoint List |
| 📅 **Event Calendar** | Live calendar with month/week view | SPFx + Graph API |
| 📊 **KPI Tracker** | Live metric cards from Power BI datasets | SPFx + Power BI Embedded |
| 👥 **Org Directory** | Searchable employee directory | SPFx + Graph API |
| 🌤 **Weather Widget** | Location-aware weather via external API | SPFx + Azure Functions |
| 📢 **Announcements** | Priority-based alert banner with dismissal | SPFx + SharePoint List |

---

### 📊 Power BI Dashboards Embedded

| Dashboard | Department | KPIs Tracked |
|---|---|---|
| Finance | Finance | Budget vs Actuals, Spend Trends |
| People | HR | Headcount, Attrition, Leave |
| Support | IT | Ticket Volume, SLA Compliance |
| Delivery | Operations | Project Status, KPIs |
| Revenue | Sales | Pipeline, Targets, Regional |

---

### 🏗️ Architecture

```
SharePoint Online
│
├── SPFx Web Parts (React + TypeScript + Fluent UI)
│   ├── News Feed ────────────── SharePoint List (REST)
│   ├── KPI Tracker ──────────── Power BI Embedded
│   ├── Org Directory ─────────── Microsoft Graph API
│   └── Event Calendar ────────── Graph API /events
│
├── Azure Functions (serverless backend)
│   └── Weather API · 3rd-party KPI integrations
│
└── PnP JS / REST API
    └── List & Library CRUD operations
```

</td>

<!-- RIGHT COLUMN -->
<td width="35%">

### 📌 Project Details

| | |
|---|---|
| **Type** | Intranet Modernization |
| **Platform** | SharePoint Online |
| **Users** | 500+ daily |
| **Duration** | Full lifecycle |
| **Role** | SharePoint Developer |
| **Status** | ✅ Live |

---

### 🛠️ Tech Stack

![SharePoint](https://img.shields.io/badge/SharePoint_Online-0078D4?style=flat-square&logo=microsoft-sharepoint&logoColor=white)
![SPFx](https://img.shields.io/badge/SPFx-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Fluent UI](https://img.shields.io/badge/Fluent_UI-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Graph API](https://img.shields.io/badge/MS_Graph-00BCF2?style=flat-square&logo=microsoft&logoColor=white)
![Azure Functions](https://img.shields.io/badge/Azure_Functions-0062AD?style=flat-square&logo=azure-functions&logoColor=white)
![PnP JS](https://img.shields.io/badge/PnP_JS-green?style=flat-square)

---

### 📈 Results

| Metric | Outcome |
|---|---|
| Page load | ~40% faster |
| Engagement | +65% in 60 days |
| BI reporting | Live dashboards |
| Self-service | Full adoption |

---

### 🔐 Governance

- RBAC across all site collections
- Audience targeting per dept
- Content approval for news
- Retention policies on libs

</td>
</tr>
</table>

---
 
## 📁 Project Structure
 
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
 
<div align="center">

<table width="100%">
<tr>
<td align="center" style="padding:12px; background:#f3f2f1;">

**Bobba S Jaswanth Chowdary** · SharePoint Developer · India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jaswanthchowdarybobba/)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:bobbajaswanthchowdary@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/jaswanthchowdarybobba)

</td>
</tr>
</table>

</div>
