# Project Intake Form

**Purpose:** Fill this document BEFORE starting development to provide AI agents with essential context
**Status:** [TEMPLATE - Fill before first sprint]
**Last Updated:** [DATE]

---

## 🎯 Project Overview

### 1. What does this application do?
**Describe in 1-3 sentences what users will do with this app:**

[ОТВЕТИТЬ: Например, "Это приложение для управления задачами, где пользователи могут создавать проекты, добавлять задачи, назначать их членам команды и отслеживать прогресс в реальном времени."]

---

### 2. Who are the users?
**Target audience:**

[ОТВЕТИТЬ: Например, "Малые команды (3-10 человек), фрилансеры, студенты"]

---

### 3. Main problem this solves
**What pain point does this address?**

[ОТВЕТИТЬ: Например, "Существующие task-менеджеры слишком сложные для малых команд и дорогие"]

---

## 🛠️ Technology Stack

### 4. Frontend Framework
**Choose one and specify version if important:**

- [ ] React (with Next.js / Vite / CRA)
- [ ] Vue.js (with Nuxt / Vite)
- [ ] Angular
- [ ] Svelte / SvelteKit
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ: Например, "React 18 + Next.js 14 (App Router)"]

---

### 5. Language
**TypeScript or JavaScript?**

- [ ] TypeScript (recommended)
- [ ] JavaScript

**Selected:** [ОТВЕТИТЬ]

---

### 6. Styling Solution

- [ ] Tailwind CSS (recommended for speed)
- [ ] CSS Modules
- [ ] Styled Components / Emotion
- [ ] Plain CSS / SCSS
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

### 7. Backend / Database

**Choose backend approach:**

- [ ] Supabase (recommended - auth + DB + real-time)
- [ ] Firebase
- [ ] Custom backend (Node.js / Python / Go)
- [ ] Serverless (AWS Lambda / Vercel Functions)
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

**Database type:**
- [ ] PostgreSQL (Supabase)
- [ ] MongoDB
- [ ] MySQL
- [ ] SQLite
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

### 8. Authentication

**How will users log in?**

- [ ] Email/Password
- [ ] OAuth (Google, GitHub, etc.)
- [ ] Magic Link (passwordless)
- [ ] Phone (SMS)
- [ ] No auth needed
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

**Auth provider:**
- [ ] Supabase Auth
- [ ] Firebase Auth
- [ ] Auth0
- [ ] NextAuth.js
- [ ] Custom
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

### 9. Hosting / Deployment

**Where will this be deployed?**

- [ ] Vercel (recommended for Next.js)
- [ ] Netlify
- [ ] AWS
- [ ] Google Cloud
- [ ] Self-hosted
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

## ✨ Core Features (MVP)

### 10. List 3-5 main features for MVP

**Priority order (most important first):**

1. [ОТВЕТИТЬ: Например, "User registration and authentication"]
2. [ОТВЕТИТЬ: Например, "Create and manage projects"]
3. [ОТВЕТИТЬ: Например, "Add tasks to projects with due dates"]
4. [ОТВЕТИТЬ: Например, "Invite team members to projects"]
5. [ОТВЕТИТЬ: Например, "Real-time updates when tasks change"]

---

### 11. User Roles

**Does the app have different user types?**

- [ ] No roles (all users equal)
- [ ] Yes, multiple roles

**If yes, list roles:**
- [ОТВЕТИТЬ: Например, "Admin - full access"]
- [ОТВЕТИТЬ: Например, "Team Member - can view and edit tasks"]
- [ОТВЕТИТЬ: Например, "Viewer - read-only access"]

---

## 📊 Data Structure

### 12. Main Entities (Database Tables)

**List main data models and their key fields:**

**Example:**
```
Users
  - id, email, name, avatar, role, created_at

Projects
  - id, title, description, owner_id, created_at

Tasks
  - id, title, description, project_id, assignee_id, due_date, status
```

**Your entities:**
```
[ОТВЕТИТЬ: Перечислить основные таблицы и их поля]

Entity 1: [Name]
  - [field1], [field2], [field3]...

Entity 2: [Name]
  - [field1], [field2], [field3]...

Entity 3: [Name]
  - [field1], [field2], [field3]...
```

---

### 13. Relationships

**How are entities connected?**

[ОТВЕТИТЬ: Например,
- "One User can own many Projects (1:N)"
- "One Project can have many Tasks (1:N)"
- "One Task belongs to one User (assignee) (N:1)"
- "Users and Projects - many-to-many (team members)"]

---

## 🔌 External Integrations

### 14. Third-Party Services

**Will the app integrate with external services?**

- [ ] Email service (SendGrid, Resend, Mailgun)
- [ ] Payment processing (Stripe, PayPal)
- [ ] File storage (AWS S3, Cloudinary)
- [ ] Analytics (Google Analytics, Plausible)
- [ ] AI/ML services (OpenAI, Anthropic)
- [ ] Other: [УКАЗАТЬ]

**Selected integrations:**
[ОТВЕТИТЬ: Список сервисов с кратким описанием зачем]

---

### 15. API Requirements

**Does the app need to expose an API?**

- [ ] No, frontend only
- [ ] Yes, REST API
- [ ] Yes, GraphQL
- [ ] Yes, WebSocket / Real-time

**If yes, describe:**
[ОТВЕТИТЬ: Например, "REST API для мобильного приложения в будущем"]

---

## 🎨 UI/UX Requirements

### 16. Design Reference

**Are there existing apps with similar UI?**

[ОТВЕТИТЬ: Например,
- "Linear.app - минималистичный, быстрый"
- "Notion - гибкий, модульный"
- "Slack - современный, дружелюбный"]

---

### 17. Design Assets Available?

**Do you have designs ready?**

- [ ] Yes, Figma/Sketch designs available
  - Link: [ВСТАВИТЬ ССЫЛКУ]
- [ ] Yes, screenshots/wireframes
  - Location: [УКАЗАТЬ ГДЕ]
- [ ] No, AI should propose basic UI
- [ ] No, will design as we go

**Selected:** [ОТВЕТИТЬ]

---

### 18. Responsive Requirements

**Mobile support needed?**

- [ ] Desktop only
- [ ] Responsive (mobile + desktop)
- [ ] Mobile-first
- [ ] Native mobile app planned later

**Selected:** [ОТВЕТИТЬ]

---

## 🔐 Security & Compliance

### 19. Security Requirements

**Any special security needs?**

- [ ] Standard web security (XSS, CSRF protection)
- [ ] GDPR compliance required
- [ ] HIPAA compliance (healthcare data)
- [ ] PCI compliance (payment data)
- [ ] Two-factor authentication (2FA)
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

### 20. Data Privacy

**Where should data be stored?**

- [ ] Any region (no restrictions)
- [ ] EU only (GDPR)
- [ ] US only
- [ ] Specific region: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

## 📈 Scale & Performance

### 21. Expected Scale

**How many users expected in first year?**

- [ ] < 100 users (prototype/MVP)
- [ ] 100-1,000 users (small app)
- [ ] 1,000-10,000 users (growing app)
- [ ] 10,000+ users (production scale)

**Selected:** [ОТВЕТИТЬ]

---

### 22. Performance Requirements

**Any critical performance needs?**

[ОТВЕТИТЬ: Например,
- "Page load < 2 seconds"
- "Real-time updates < 500ms delay"
- "Support 1000 concurrent users"]

---

## 💰 Budget & Timeline

### 23. Development Timeline

**Expected timeline for MVP?**

- [ ] 1-2 weeks (simple MVP)
- [ ] 1 month (standard MVP)
- [ ] 2-3 months (complex MVP)
- [ ] Other: [УКАЗАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

### 24. Budget Constraints

**Any constraints on external services cost?**

[ОТВЕТИТЬ: Например, "Стараться использовать free tier сервисов, платные только если критично"]

---

## 🔄 Development Approach

### 25. Development Style

**Preferred approach:**

- [ ] Start with complete architecture planning, then code
- [ ] Iterative - build feature by feature
- [ ] Rapid prototyping - get working version fast, refine later

**Selected:** [ОТВЕТИТЬ]

---

### 26. Testing Requirements

**Testing strategy:**

- [ ] Manual testing only (dev environment)
- [ ] Unit tests for critical functions
- [ ] Integration tests
- [ ] E2E tests (Playwright, Cypress)
- [ ] No tests for MVP

**Selected:** [ОТВЕТИТЬ]

---

## 📚 Reference Materials

### 27. Similar Projects

**Are there similar projects for reference?**

[ОТВЕТИТЬ: Например, "У меня есть проект MainChatMemory по адресу /path/to/project - можно взять оттуда паттерны"]

---

### 28. Existing Codebase

**Starting from scratch or existing code?**

- [ ] From scratch (new project)
- [ ] Existing codebase to extend
  - Location: [УКАЗАТЬ ПУТЬ]
  - What needs to be added: [ОПИСАТЬ]

**Selected:** [ОТВЕТИТЬ]

---

## 🎯 Success Criteria

### 29. MVP Definition of Done

**What makes this MVP complete?**

[ОТВЕТИТЬ: Список критериев, например:
- [ ] User can register and log in
- [ ] User can create projects
- [ ] User can add tasks to projects
- [ ] User can invite team members
- [ ] Real-time updates work
- [ ] App deployed to production
- [ ] No critical bugs]

---

### 30. Post-MVP Plans

**What comes after MVP?**

[ОТВЕТИТЬ: Например,
- "Add mobile app (React Native)"
- "Add advanced analytics"
- "Add integrations with Slack, Telegram"]

---

## 📝 Additional Notes

### 31. Special Requirements or Constraints

**Anything else AI should know?**

[ОТВЕТИТЬ: Любые дополнительные требования, ограничения, пожелания]

---

## ✅ Completion Checklist

**Before starting development, ensure:**

- [ ] All sections marked with [ОТВЕТИТЬ] are filled
- [ ] Technology stack is clearly defined
- [ ] MVP features are prioritized
- [ ] Data structure is outlined
- [ ] Reference materials are provided (if any)
- [ ] This file is committed to git
- [ ] BACKLOG.md is updated with initial features
- [ ] ARCHITECTURE.md is updated with tech stack

---

## 🚀 Next Steps After Filling This Form

1. **AI Agent reads this file** to understand project context
2. **Update BACKLOG.md** - add MVP features to "Planned" section
3. **Update ARCHITECTURE.md** - document chosen tech stack
4. **Start first sprint** - begin with highest priority feature
5. **Follow WORKFLOW.md** - use sprint completion checklist

---

## 📋 Template Version

**Version:** 1.0
**Last Updated:** [DATE]
**Maintained by:** AI Agent + Project Lead

---

*This intake form ensures AI agents have all necessary context to start development efficiently*
*Fill once per project, update as requirements evolve*
