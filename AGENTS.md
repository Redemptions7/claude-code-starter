# AI Agent Instructions

**Project:** [PROJECT_NAME]
**Purpose:** Meta-instructions for effective AI-assisted development
**Created:** [DATE]
**Last Updated:** [DATE]

> **Note:** This file is optimized for AI assistants (Claude Code, Cursor, Copilot, etc.) working with this codebase.

---

## 🎯 Quick Start for AI Agents

### Required Reading (in order):
1. **SECURITY.md** - Security requirements and practices (READ FIRST!)
2. **ARCHITECTURE.md** - System architecture and technical decisions
3. **BACKLOG.md** - Current implementation status and roadmap (SINGLE SOURCE OF TRUTH)
4. **README.md** - User-facing project information
5. **WORKFLOW.md** - Development processes and sprint workflow

### ⚠️ SINGLE SOURCE OF TRUTH:
**BACKLOG.md** is the ONLY authoritative source for:
- Current implementation status
- Feature priorities
- Development roadmap

### Key Files Quick Reference:
```bash
# Architecture & Planning
ARCHITECTURE.md                # System design and patterns
BACKLOG.md                     # Implementation status (SINGLE SOURCE OF TRUTH)
WORKFLOW.md                    # Development processes
README.md                      # User-facing documentation

# Core Application
[ЗАПОЛНИТЬ: основные файлы проекта]
# Например:
# src/store/useStore.ts        # State management
# src/lib/api.ts               # API service
# src/components/Main.tsx      # Main component

# Configuration
.claude/commands/              # Custom slash commands for Claude Code
.claudeignore                  # Files to ignore in AI context
```

---

## 📚 Technology Stack

### Frontend
[ЗАПОЛНИТЬ: Frontend технологии]
```
- Framework: [React/Vue/Angular/Next.js/etc]
- Language: [TypeScript/JavaScript]
- State Management: [Redux/Zustand/Context/etc]
- Styling: [Tailwind/CSS Modules/Styled Components/etc]
- Build Tool: [Vite/Webpack/Next.js/etc]
```

### Backend & Infrastructure
[ЗАПОЛНИТЬ: Backend технологии]
```
- Database: [PostgreSQL/MySQL/MongoDB/etc]
- Authentication: [Supabase Auth/Auth0/Firebase/etc]
- API: [REST/GraphQL/tRPC/etc]
- Hosting: [Vercel/AWS/etc]
```

### Key Dependencies
```json
{
  "[ЗАПОЛНИТЬ]": "версия и назначение",
}
```

---

## 🚫 NEVER DO

### Code & Architecture
- ❌ **[ЗАПОЛНИТЬ: специфичные для проекта правила]**
- ❌ **Update database structure** without migration script
- ❌ **Use `any` type** without explicit justification (TypeScript projects)
- ❌ **Create multiple components in one file** (если используется компонентный подход)
- ❌ **Duplicate API calls** (especially in polling loops)
- ❌ **Ignore security best practices** (SQL injection, XSS, CSRF)

### Process & Documentation
- ❌ **Skip documentation updates** after sprint completion
- ❌ **Modify BACKLOG.md** without completing actual implementation
- ❌ **Create commits** without meaningful messages
- ❌ **Update dependencies** without testing
- ❌ **Push to main/master** without review (if team workflow requires it)

### 🔐 Security (CRITICAL - NEVER COMPROMISE)
- ❌ **NEVER hardcode secrets** (API keys, passwords, tokens) in code
- ❌ **NEVER commit `.env` or `.env.local`** to repository
- ❌ **NEVER trust user input** - always validate and sanitize
- ❌ **NEVER use `eval()` or `new Function()`** with user data
- ❌ **NEVER expose sensitive data** in error messages or logs
- ❌ **NEVER skip input validation** on server-side (client-side is not enough!)
- ❌ **NEVER create SQL queries** with string concatenation (use parameterized)
- ❌ **NEVER disable security features** (CORS, CSRF protection, etc)
- ❌ **NEVER deploy without** running security checks (npm audit, secret scan)
- ❌ **NEVER assume data is safe** - sanitize output to prevent XSS

---

## ✅ ALWAYS DO

### Before Making Changes
- ✅ **Read ARCHITECTURE.md** for architectural decisions
- ✅ **Check BACKLOG.md** for current status
- ✅ **Review related documentation** before making changes
- ✅ **Test in development** environment first

### During Development
- ✅ **Use existing patterns** from codebase
- ✅ **Follow TypeScript strict mode** (type everything properly)
- ✅ **Write migration scripts** for database changes
- ✅ **Update types** after schema changes
- ✅ **Test thoroughly** before marking tasks as complete
- ✅ **Use TodoWrite tool** to track progress

### 🔐 Security (Every Single Time)
- ✅ **READ SECURITY.md** before starting ANY coding task
- ✅ **Validate ALL user input** (type, format, length, range)
- ✅ **Sanitize ALL output** (prevent XSS attacks)
- ✅ **Use environment variables** for ALL secrets (never hardcode)
- ✅ **Use parameterized queries** for database (prevent SQL injection)
- ✅ **Check authentication** before accessing protected resources
- ✅ **Check authorization** (user has permission for this action?)
- ✅ **Handle errors securely** (log internally, show generic message to user)
- ✅ **Run npm audit** before committing changes
- ✅ **Review SECURITY.md checklist** for current development stage
- ✅ **Think like an attacker** - "How could I break this?"

### After Completion
- ✅ **Update BACKLOG.md** with implementation status
- ✅ **Update ARCHITECTURE.md** if architectural changes made
- ✅ **Update AGENTS.md** if new patterns/rules discovered
- ✅ **Update README.md** if user-facing changes
- ✅ **Create meaningful git commit** (see WORKFLOW.md for template)
- ✅ **Mark all TodoWrite tasks** as completed

---

## 🔧 Standard Workflows

### Database Changes
```
1. Analysis → Read current database schema/documentation
2. Planning → Create migration script
3. Testing → Apply migration in development
4. Type Update → Update TypeScript types (if applicable)
5. Documentation → Update ARCHITECTURE.md or database docs
6. Code → Implement feature using new schema
7. Sprint Completion → Update BACKLOG.md and AGENTS.md
```

### New Feature Development
```
1. Read ARCHITECTURE.md (understand patterns)
2. Check BACKLOG.md (current status)
3. Plan with TodoWrite tool
4. Implement following existing patterns
5. Test thoroughly
6. Update documentation (BACKLOG.md, AGENTS.md, README.md)
7. Create sprint completion commit
```

### Bug Fix
```
1. Diagnose root cause
2. Check if similar issue exists in AGENTS.md "Common Issues"
3. Fix following existing patterns
4. Test fix
5. Add to "Common Issues" section if applicable
6. Update version in README.md if necessary
```

### 🔐 Security Review (Before Every Deploy)
```
1. Read SECURITY.md - Review all checklists
2. Run npm audit - Fix high/critical vulnerabilities
3. Scan for secrets - grep for API keys, tokens, passwords
4. Test authentication - Try bypassing auth if applicable
5. Test authorization - Try accessing other users' data
6. Test input validation - Send malicious input (XSS, injection)
7. Review error handling - Ensure no sensitive data exposed
8. Check environment variables - All secrets server-side only
9. Verify HTTPS enforced - Production uses HTTPS
10. Complete Security Sign-Off - Use template from SECURITY.md
```

---

## 🏗️ Architectural Patterns

[ЗАПОЛНИТЬ: Специфичные для проекта архитектурные решения]

### Примеры паттернов для заполнения:

#### State Management Pattern
**Decision:** [Redux/Zustand/Context/etc]
**Reason:**
- [Причина 1]
- [Причина 2]

**Example:**
```typescript
// Пример использования
```

#### API Integration Pattern
**Decision:** [Как организованы API запросы]
**Reason:**
- [Причина 1]

#### File/Data Structure Pattern
**Decision:** [Как организованы данные]
**Reason:**
- [Причина 1]

---

## 🐛 Common Issues & Solutions

[ЗАПОЛНИТЬ по мере обнаружения проблем]

### Issue: [Название проблемы]
**Symptom:** [Описание симптома]
**Root Cause:** [Причина]
**Solution:** [Решение]
**File:** [Где исправлять]

### Template для добавления:
```markdown
### Issue: [Название]
**Symptom:** [Что видит пользователь/разработчик]
**Root Cause:** [Почему происходит]
**Solution:** [Как исправить]
**File:** [Где находится код]
```

---

## 📋 Task Checklists

### Adding New Feature
- [ ] Read ARCHITECTURE.md and BACKLOG.md
- [ ] Create TodoWrite task list
- [ ] Implement following existing patterns
- [ ] Write/update tests
- [ ] Update TypeScript types (if applicable)
- [ ] Update UI components
- [ ] Update BACKLOG.md status
- [ ] Update ARCHITECTURE.md (if architectural changes)
- [ ] Update README.md (if user-facing changes)
- [ ] Create sprint completion commit

### Database Schema Change
- [ ] Create migration script
- [ ] Test in development environment
- [ ] Update TypeScript types/interfaces
- [ ] Update database documentation
- [ ] Update related code
- [ ] Test all affected features
- [ ] Update ARCHITECTURE.md
- [ ] Update BACKLOG.md status
- [ ] Create sprint completion commit

### Bug Fix
- [ ] Reproduce and document bug
- [ ] Identify root cause
- [ ] Implement fix
- [ ] Test fix thoroughly
- [ ] Check for similar issues elsewhere
- [ ] Add to "Common Issues" (if applicable)
- [ ] Update BACKLOG.md (if tracked)
- [ ] Create fix commit

---

## 🔍 Debugging Quick Reference

### [ЗАПОЛНИТЬ: Специфичные команды для отладки]

```bash
# Database debugging
[команды для проверки БД]

# API debugging
[команды для проверки API]

# State debugging
[команды для проверки состояния]
```

---

## 📊 Performance Guidelines

### [ЗАПОЛНИТЬ: Специфичные для проекта]

**API Optimization:**
- [Правило 1]
- [Правило 2]

**Database Performance:**
- [Правило 1]
- [Правило 2]

**Frontend Performance:**
- [Правило 1]
- [Правило 2]

---

## 🚀 Code Templates

### [ЗАПОЛНИТЬ: Шаблоны кода для проекта]

#### New Component Template
```typescript
// Пример шаблона компонента
```

#### New API Route Template
```typescript
// Пример шаблона API route
```

#### New Service Method Template
```typescript
// Пример шаблона метода сервиса
```

---

## 📝 Sprint Workflow

See **WORKFLOW.md** for detailed sprint processes, including:
- Sprint structure and phases
- Completion checklists
- Commit message templates
- Documentation update requirements

**Key Rule:** NEVER end a sprint without updating all relevant documentation files.

---

## 🔄 Version History

- **[DATE]:** Initial template created
- [Добавляйте записи по мере развития проекта]

---

## 📝 Notes for Customization

Когда заполняете этот файл для конкретного проекта:

1. **Замените [ЗАПОЛНИТЬ]** на актуальную информацию
2. **Удалите эту секцию** после заполнения
3. **Добавляйте новые секции** по мере необходимости
4. **Обновляйте** после каждого спринта
5. **Документируйте паттерны** которые появляются в проекте
6. **Добавляйте в Common Issues** решенные проблемы

---

*This file should be updated after every sprint completion*
*Goal: Maintain living documentation for effective AI-assisted development*
*Compatible with: Claude Code, Cursor, GitHub Copilot, and other AI coding assistants*
