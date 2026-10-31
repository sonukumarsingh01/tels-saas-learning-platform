<div align="center">

# 🚀 TELS — TitanEd Learning Services

### A subscription SaaS learning platform built on Open edX

**Product owner:** TitanEd (about the company: [Open edX marketplace listing](https://openedx.org/marketplace/titaned/)) &nbsp;·&nbsp; **My role:** Frontend Engineer at TitanEd &nbsp;·&nbsp; **Aug 2025 – Present**

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat&logo=redux&logoColor=white)
![Open edX](https://img.shields.io/badge/Open%20edX-02262B?style=flat)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat&logo=sentry&logoColor=white)

</div>

> **Note:** TELS is a commercial product and its source code is private. This repository is a **project showcase**: it explains
> the business problem, my contribution and how it was built. It contains no company code.

> 🔗 **About the links:** client links go to the **client's own official website**, for reference only. Those sites were **not built by me**. My work is the private learning platform described below.

---

## 📌 The business problem

TitanEd sells a ready-to-use learning platform to organisations **by subscription**. The platform is built on Open edX, the
open-source LMS behind edX.org, but standard Open edX:

- looks dated and is hard to brand for each customer
- gives instructors few tools to plan and track their teaching
- has no AI
- needed weeks of custom frontend work for every new customer

## ✅ My contribution

As part of the TitanEd team, I worked on the **custom user interface of TELS**: the learner site (LMS), the course-authoring site (Studio/CMS) and all
**11 Open edX micro-frontend apps**. I also added features that standard Open edX doesn't have.

| Capability | What it does for the business |
|---|---|
| 🎨 **Ready-made platform templates** (Native, Template A, Template B) | A new subscriber picks a template and brands it. No custom development per customer |
| 🧩 **No-code theming with design tokens** | Admins change colours, fonts, sizes and every component from the admin panel ([details](https://github.com/sonukumarsingh01/openedx-design-token-theming)) |
| 🤖 **TELS AI assistant** | AI help for learners and admins in every app ([details](https://github.com/sonukumarsingh01/tels-ai-openedx-assistant)) |
| 📅 **Instructor dashboard** | Calendar, assignments, widgets and graphs: an instructor's whole workload in one place |
| 🌐 **Multilingual public marketing website** | Each customer gets a branded landing site connected to live course data |
| 📣 **Announcement banners and in-app feedback** | Platform-wide messages and direct user feedback, from a shared component library |
| 🔁 **Old/new interface switch** | Customers move to the new interface at their own pace, so rollouts are safer |
| 🧭 **One shared header and footer** | All 11 apps feel like one product, with search and a custom user menu |
| ⬆️ **Upgrade to the latest Open edX release (Verawood)** | All 11 apps upgraded through plugins, with no forks, so future upgrades stay cheap |
| 🛡️ **Sentry error monitoring** | Production errors are caught before customers report them |

## 📈 Business impact

- **Faster sales-to-launch:** a new customer launches by configuration instead of a development project.
- **Lower cost per customer:** one codebase serves every subscriber.
- **Upgrade-safe:** everything ships through Open edX plugin slots and Tutor plugins, never forks.
- **More to sell:** AI and no-code branding are built in, and both are also sold separately to standard Open edX clients.

## 🏗️ How it's built

```
          ┌──────────────────────────── TELS ────────────────────────────┐
 Learner ─┤  Learning · Dashboard · Profile · Account · Discussions      │
          │  Public marketing site (multilingual)                        │
 Teacher ─┤  Studio (Authoring) + AI Assistant + Instructor dashboard     │
          │  Gradebook · ORA Grading · Communications                    │
          ├───────────────────────────────────────────────────────────────┤
          │  Shared header/footer (Tutor plugin) · Design tokens · Banners │
          │  TELS AI plugin · Sentry                                       │
          ├───────────────────────────────────────────────────────────────┤
          │  Open edX (Verawood) · Tutor · Docker                          │
          └───────────────────────────────────────────────────────────────┘
```

- **Frontend:** React, TypeScript, Redux, Paragon (the Open edX design system), SCSS
- **Extension approach:** Frontend Plugin Framework slots, Tutor plugins, a shared TypeScript component library
- **Platform:** Open edX (Verawood), Tutor, Docker on Ubuntu
- **Quality:** Sentry, Jest, React Testing Library

## 👤 My role

Frontend Engineer on the TELS team: worked on the custom apps, templates and shared components, delivered features from
design to production with the backend and product teams, and helped with Open edX upgrades. About 140 pull requests on this product.

---

<div align="center">

**Sonu Kumar** · Frontend Engineer · [LinkedIn](https://www.linkedin.com/in/dr-sonu-kumar/) · [GitHub](https://github.com/sonukumarsingh01)

</div>
