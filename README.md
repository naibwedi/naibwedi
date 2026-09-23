<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:14100A,100:C9963A&height=190&section=header&text=Naibe%20Mehari%20Tekle&fontSize=44&fontColor=F3E6C8&fontAlignY=38&desc=ሰላም%20%E2%80%94%20Software%20Engineer&descSize=20&descColor=F3E6C8&descAlignY=60" width="100%" alt="Naibe Mehari Tekle — Software Engineer" />

<a href="https://naibtech.dev">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=19&pause=1200&color=C9963A&center=true&vCenter=true&width=720&lines=Industrial+software+in+C%23+%2F+.NET;Speech+AI+for+Tigrinya+%26+Amharic;Interpretable+ML+%E2%80%94+Tsetlin+Machines;Immersive+3D+on+the+web" alt="Typing SVG" />
</a>

[![Portfolio](https://img.shields.io/badge/Portfolio-naibtech.dev-C9963A?style=for-the-badge&labelColor=14100A)](https://naibtech.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/naib-mehari-95690114a/)
[![Email](https://img.shields.io/badge/Email-naibmehari%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:naibmehari@gmail.com)
[![CV](https://img.shields.io/badge/CV-Download_PDF-14100A?style=for-the-badge&labelColor=C9963A&color=14100A)](https://naibtech.dev/Naibe-Mehari-CV.pdf)

![Open to work](https://img.shields.io/badge/Open_to_work-Full--time_engineering_roles-2E7D32?style=flat-square)
![Based in](https://img.shields.io/badge/Based_in-Norway-14100A?style=flat-square)
![Languages](https://img.shields.io/badge/Speaks-Norsk_·_English_·_ትግርኛ_·_العربية-C9963A?style=flat-square&labelColor=14100A)

<br>

[**About**](#-about) · [**Flagship**](#-flagship-habeshavoice-studio) · [**Projects**](#-projects) · [**Stack**](#-stack) · [**Stats**](#-stats) · [**Contact**](#-contact)

</div>

---

## 👋 About

I'm a software engineer finishing my B.Eng. in Computer Engineering at the **University of Agder**, and I currently build industrial software at **Red Rock** — a live PLC data tool in C# / .NET 8 on Avalonia and Beckhoff TwinCAT ADS.

Outside work I build things nobody handed me a spec for: a speech studio for my own language, an interpretable-ML research lab, and a 3D walk through a church I'd love people to see.

```csharp
var naibe = new Engineer
{
    DayJob    = "Industrial software @ Red Rock — Avalonia · ReactiveUI · TwinCAT ADS",
    Nights    = new[] { "Speech AI (Tigrinya/Amharic)", "Tsetlin Machine research", "Three.js" },
    Backbone  = new[] { "C# / .NET 8", "TypeScript", "Python" },
    Tongues   = new[] { "Norsk", "English", "ትግርኛ", "العربية" },
    Likes     = "Systems that are tested, explainable, and finished.",
};
```

---

## 🎙️ Flagship: HabeshaVoice Studio

> A private speech-to-text workspace for **Tigrinya and Amharic** — languages that mainstream tools barely support.

[**Source →**](https://github.com/naibwedi/habeshavoice-studio)

- **Record or upload**, listen back, then transcribe — audio leaves the browser only after explicit consent
- **Review workflow** — edit the working transcript while the original machine transcript is kept for reference
- **Private library** — searchable sessions, export to TXT / Markdown / PDF
- **Split architecture** — web app on a standard host, GPU inference in a separate FastAPI service; the service credential never reaches the browser

```mermaid
flowchart LR
    B["Browser<br/>record · review · export"] --> W["Next.js app<br/>auth + library"]
    W --> A["Authenticated API routes"]
    A --> S["FastAPI service<br/>Ethio-ASR on GPU"]
    A --> D[("Private transcripts<br/>+ audio in Vercel Blob")]
```

`Next.js` · `TypeScript` · `FastAPI` · `Python` · `Vercel Blob` · `CI: typecheck + test + build`

---

## 🚀 Projects

### 🧠 AI & Machine Learning

| Project | What it is | Stack | Links |
|---|---|---|---|
| **HabeshaVoice Studio** | Speech-to-text product for Tigrinya & Amharic | Next.js · FastAPI · Ethio-ASR | [Source](https://github.com/naibwedi/habeshavoice-studio) |
| **Tsetlin Market Lab** | Predicts the *next bookmaker price move* with a Tsetlin Machine vs XGBoost/LightGBM baselines — leakage-safe, time-ordered splits, cron-collected data, human-readable clauses. Research, not betting tips. | Python · tmu · GitHub Actions | [Source](https://github.com/naibwedi/tsetlin-market-lab) |
| **LogicAlpha** | Purged walk-forward strategy selection with Boolean features, cost-aware backtests and an optional Tsetlin Machine | Python | [Source](https://github.com/naibwedi/logic-alpha-tm) |
| **CampusCart** | Student marketplace whose uploads pass a Cloud Vision moderation pipeline that deletes flagged images and notifies the seller | React Native · Firebase · Cloud Functions | [Source](https://github.com/naibwedi/Campus-Cart-App) |

### 🌐 Web & Creative

| Project | What it is | Stack | Links |
|---|---|---|---|
| **Selam — A Sacred Journey** | Walk from a courtyard into an Eritrean Orthodox-inspired church: guided tour, candlelight mode, ambient sound, reduced-motion option | Three.js · Web Audio | [Live](https://eritrea-sacred-journey.vercel.app) · [Source](https://github.com/naibwedi/eritrea-sacred-journey) |
| **Tigrigna → Latin** | Geez (ግዕዝ) script and numerals to Latin, client-side | HTML · CSS · JS | [Live](https://tigrigna-latin.netlify.app/) · [Source](https://github.com/naibwedi/Tigrigna-to-latin-traslator) |
| **This portfolio** | Hand-written, no framework, respects reduced-motion | HTML · CSS · JS | [Live](https://naibtech.dev) · [Source](https://github.com/naibwedi/naibe-portfolio) |

### 🖥️ Backend, Desktop & Mobile

| Project | What it is | Stack | Links |
|---|---|---|---|
| **Logi-Track** | Logistics platform — four roles, trip lifecycle, live status via SignalR, Identity, Swagger, Docker | ASP.NET Core · EF Core · SignalR | [Source](https://github.com/naibwedi/Logi-Track) |
| **FlowLingo** | Android translation keyboard — native Kotlin IME plus Flutter settings shell | Kotlin · Flutter | [Source](https://github.com/naibwedi/FlowLingo) |
| **Student Assessment App** | Grade & assessment tracking for teachers | React Native · Firebase | [Source](https://github.com/naibwedi/Student-Assesment-App) |
| **ADS Parameter Tool** | Reads live PLC symbols over TwinCAT ADS and visualises them (Red Rock — private) | C# · Avalonia · ReactiveUI | — |

### ⚙️ Systems & Fundamentals

| Project | What it is | Links |
|---|---|---|
| **x86 OS from scratch** | Bootloader, interrupts, memory management (UiA IKT218) | [Source](https://github.com/naibwedi/2025-ikt218-osdev) |
| **Mbed OS embedded** | Microcontroller I/O and real-time tasks | [Source](https://github.com/naibwedi/Mbed-OS-project-) |
| **Infix → Postfix** | Stack-based expression evaluator with trig, log, variables | [Source](https://github.com/naibwedi/infix-to-postfix-converter) |

---

## 🛠️ Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=cs,dotnet,ts,react,py,fastapi,nextjs,docker,postgres,flutter,kotlin,threejs,githubactions,git&theme=dark&perline=7" alt="Tech stack icons" />

</div>

| | |
|---|---|
| **Languages** | C#, TypeScript, Python, C++, C, JavaScript, Dart, Kotlin |
| **Backend** | ASP.NET Core, EF Core, SignalR, FastAPI, Flask, REST |
| **Frontend / Mobile** | React, Next.js, React Native, Expo, Flutter, Three.js |
| **Industrial / Desktop** | Avalonia UI, ReactiveUI (MVVM), Beckhoff TwinCAT ADS |
| **Data & ML** | Tsetlin Machines, scikit-learn, XGBoost, LightGBM, leakage-safe pipelines |
| **Ops** | Docker, GitHub Actions, GitLab CI, Vercel |

---

## 📊 Stats

<div align="center">

<img src="https://github-stats-extended.vercel.app/api?username=naibwedi&show_icons=true&hide_border=true&bg_color=14100A&title_color=C9963A&text_color=E8DCC0&icon_color=C9963A" width="48%" alt="GitHub stats" />
<img src="https://github-stats-extended.vercel.app/api/top-langs/?username=naibwedi&layout=compact&hide_border=true&bg_color=14100A&title_color=C9963A&text_color=E8DCC0" width="48%" alt="Top languages" />

</div>

---

## 📫 Contact

Open to full-time software engineering roles — especially C#/.NET, full-stack, or applied AI.

**[naibtech.dev](https://naibtech.dev)** · **[LinkedIn](https://www.linkedin.com/in/naib-mehari-95690114a/)** · **naibmehari@gmail.com**

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:C9963A,100:14100A&height=90&section=footer" width="100%" alt="" />
</div>
