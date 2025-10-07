# Project Architecture

**Project:** [PROJECT_NAME]
**Version:** [0.1.0]
**Last Updated:** [DATE]

---

## 📊 Technology Stack

### Frontend
[ЗАПОЛНИТЬ: Детали frontend стека]
```
- Framework: [React/Vue/Angular/Svelte/Next.js/etc]
- Language: [TypeScript/JavaScript]
- Build Tool: [Vite/Webpack/Next.js/Turbopack/etc]
- State Management: [Redux/Zustand/Context API/Pinia/etc]
- UI/CSS: [Tailwind/CSS Modules/Styled Components/MUI/etc]
- Icons: [Lucide/Heroicons/FontAwesome/etc]
- Routing: [React Router/Next Router/Vue Router/etc]
```

### Backend & Infrastructure
[ЗАПОЛНИТЬ: Детали backend стека]
```
- Database: [PostgreSQL/MySQL/MongoDB/Supabase/Firebase/etc]
- Authentication: [Supabase Auth/Auth0/Firebase Auth/NextAuth/etc]
- API Type: [REST/GraphQL/tRPC/etc]
- File Storage: [S3/Supabase Storage/Cloudinary/etc]
- Hosting: [Vercel/AWS/Netlify/Railway/etc]
```

### Key Dependencies
```json
{
  "[package-name]": "^version - [назначение]",
  "Примеры:": "",
  "react": "^18.3.1 - UI library",
  "@supabase/supabase-js": "^2.x.x - Database client",
  "zustand": "^5.x.x - State management"
}
```

---

## 🗂️ Project Structure

```
[PROJECT_NAME]/
├── [ЗАПОЛНИТЬ: структура директорий]
│
│ Примерная структура:
├── src/                      # Source code
│   ├── components/           # React/Vue components
│   │   ├── ui/              # Reusable UI components
│   │   └── features/        # Feature-specific components
│   ├── lib/                 # Libraries and utilities
│   │   ├── api.ts           # API client
│   │   ├── db.ts            # Database client
│   │   └── utils.ts         # Helper functions
│   ├── hooks/               # Custom hooks
│   ├── store/               # State management
│   ├── types/               # TypeScript types
│   ├── pages/               # Pages/Routes
│   └── App.tsx              # Root component
│
├── public/                   # Static files
├── [database-folder]/        # Database migrations/schemas
├── .env.example             # Environment variables template
├── package.json             # Dependencies
└── tsconfig.json            # TypeScript configuration
```

---

## 🏗️ Core Architecture Decisions

### 1. [Архитектурное решение #1]

**Decision:** [Что решили]
**Reasoning:**
- ✅ [Причина 1]
- ✅ [Причина 2]
- ✅ [Причина 3]

**Alternatives considered:**
- ❌ [Альтернатива 1] - [почему отвергли]
- ❌ [Альтернатива 2] - [почему отвергли]

**Implementation:**
```typescript
// Пример реализации
```

### 2. [Архитектурное решение #2]

**Decision:** [Что решили]
**Reasoning:**
- ✅ [Причина 1]
- ✅ [Причина 2]

**Alternatives considered:**
- ❌ [Альтернатива] - [почему отвергли]

---

### Template для новых решений:

```markdown
### N. [Название решения]

**Decision:** [Краткое описание решения]
**Reasoning:**
- ✅ [Преимущество 1]
- ✅ [Преимущество 2]

**Alternatives considered:**
- ❌ [Отвергнутая альтернатива] - [причина]

**Data structure/Implementation:**
[Код или структура данных]
```

---

## 🔧 Key Services & Components

### [Сервис/Компонент #1]
**Purpose:** [Назначение]
**Location:** `[путь к файлу]`

**Key methods/features:**
```typescript
- method1() → описание
- method2() → описание
- feature1 → описание
```

**Architectural features:**
- [Особенность 1]
- [Особенность 2]

**Example usage:**
```typescript
// Пример использования
```

---

### Template для документирования сервисов:

```markdown
### [Service Name]
**Purpose:** [Что делает]
**Location:** `[file path]`

**Key methods:**
- method() → [описание]

**Features:**
- [Особенность]

**Example:**
[код]
```

---

## 📡 Data Flow & Integration Patterns

### 1. [User Flow #1 - например "User Login"]
```
User Action →
├── Step 1
├── Step 2
├── Step 3
└── Final Result
```

**Detailed flow:**
1. [Шаг 1 детально]
2. [Шаг 2 детально]
3. [Шаг 3 детально]

### 2. [User Flow #2]
```
[Диаграмма потока]
```

---

### Template для документирования потоков:

```markdown
### N. [Flow Name]
[ASCII диаграмма]

**Detailed:**
1. [Шаг]
2. [Шаг]
```

---

## 🎯 Development Standards

### Code Organization
- [ЗАПОЛНИТЬ: стандарты организации кода]
- **1 component = 1 file** (если применимо)
- **Services in lib/** for reusability
- **TypeScript strict mode** - no `any` (except justified exceptions)
- **Naming:** [соглашения по именованию]

### Database Patterns
[ЗАПОЛНИТЬ: если есть база данных]
- **Primary Keys:** [UUID/Auto-increment/etc]
- **Relationships:** [как организованы связи]
- **Migrations:** [как применяются миграции]
- **Security:** [RLS/Permissions/etc]

### Error Handling
- **Try/catch** in async functions
- **User-friendly** error messages (на русском/английском)
- **Console logging** for debugging
- **Fallback states** in UI

### Performance Optimizations
- [ЗАПОЛНИТЬ: специфичные для проекта оптимизации]
- **[Оптимизация 1]**
- **[Оптимизация 2]**
- **[Оптимизация 3]**

---

## 🧩 Module Architecture

[ЗАПОЛНИТЬ: если проект разбит на модули]

### [Module Name]
**Purpose:** [Назначение модуля]

**Components:**
- `Component1` - [описание]
- `Component2` - [описание]

**Integration:**
- [Как интегрируется с остальной системой]

**Example:**
```typescript
// Пример использования модуля
```

---

## 🗄️ Database Schema

[ЗАПОЛНИТЬ: структура базы данных]

### Tables Overview
```
[table_name_1]
├── id: uuid (PK)
├── field1: type
└── field2: type

[table_name_2]
├── id: uuid (PK)
└── foreign_key: uuid (FK → table_name_1)
```

### Relationships
- [Описание связей между таблицами]

### Indexes
- [Какие индексы созданы и зачем]

### Security
- [RLS policies или другие меры безопасности]

---

## 🔐 Security Architecture

[ЗАПОЛНИТЬ: меры безопасности]

### Authentication
- **Method:** [OAuth/JWT/Session/etc]
- **Provider:** [Auth0/Supabase/Custom/etc]
- **Flow:** [Описание процесса аутентификации]

### Authorization
- **Model:** [RBAC/ABAC/Custom/etc]
- **Implementation:** [Как проверяются права доступа]

### Data Protection
- **At Rest:** [Шифрование данных]
- **In Transit:** [HTTPS/TLS]
- **API Keys:** [Как хранятся]
- **Sensitive Data:** [Как обрабатываются]

### Security Headers
```javascript
// Пример настройки security headers
```

---

## 🚀 Deployment Architecture

[ЗАПОЛНИТЬ: архитектура деплоя]

### Environments
- **Development:** [localhost/dev server]
- **Staging:** [URL/описание]
- **Production:** [URL/описание]

### CI/CD Pipeline
```
[Описание процесса деплоя]
Code → Tests → Build → Deploy
```

### Environment Variables
```env
# Required
VAR_NAME=description

# Optional
OPTIONAL_VAR=description
```

---

## 📊 State Management Architecture

[ЗАПОЛНИТЬ: как организовано управление состоянием]

### Global State
```typescript
// Структура глобального состояния
interface AppState {
  [ЗАПОЛНИТЬ]
}
```

### Local State
[Когда использовать локальное состояние]

### State Update Patterns
```typescript
// Примеры паттернов обновления состояния
```

---

## 🔄 Evolution & Migration Strategy

### Approach to Changes
1. **Document decision** in this file
2. **Database changes** → Create migration script
3. **Backward compatibility** when possible
4. **Feature flags** for experimental functionality

### Migration Pattern
```
Planning → Implementation → Testing → Documentation → Deployment
    ↓           ↓              ↓           ↓            ↓
ARCHITECTURE  Code+Tests    Manual QA   Update docs   Git push
```

### Version History
- **[VERSION]** - [DATE] - [Changes summary]
- [Добавляйте по мере развития]

---

## 📚 Related Documentation

- **BACKLOG.md** - Current implementation status and roadmap
- **AGENTS.md** - AI assistant working instructions
- **WORKFLOW.md** - Development processes and sprint workflow
- **README.md** - User-facing project information

---

## 📝 Architecture Decision Records (ADR)

[Опционально: для документирования важных архитектурных решений]

### ADR-001: [Decision Title]
**Date:** [DATE]
**Status:** [Accepted/Deprecated/Superseded]
**Context:** [Почему нужно было принять решение]
**Decision:** [Что решили]
**Consequences:** [К чему это привело]

---

## 🎨 Design Patterns Used

[ЗАПОЛНИТЬ: какие паттерны проектирования используются]

- **[Pattern Name]** - [Где используется и зачем]
- Примеры:
  - **Repository Pattern** - в `lib/repositories/`
  - **Factory Pattern** - в `lib/factories/`
  - **Observer Pattern** - в state management

---

## 📝 Notes for Customization

Когда заполняете этот файл для конкретного проекта:

1. **Замените все [ЗАПОЛНИТЬ]** на актуальную информацию
2. **Удалите секции** которые не применимы к вашему проекту
3. **Добавьте новые секции** специфичные для вашего проекта
4. **Обновляйте документ** при каждом архитектурном изменении
5. **Используйте диаграммы** где нужно (Mermaid/ASCII)
6. **Удалите эту секцию** после первичного заполнения

---

*This document maintained in current state for effective development*
*Last updated: [DATE]*
