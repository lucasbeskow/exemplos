# AI AGENTS GOVERNANCE

## Project Context
Enterprise ERP SaaS
Angular v21 migration from legacy systems

---

## Source of Truth

- UI components: /libs/ui
- Design tokens: /libs/tokens
- Documentation: /docs
- Figma: MCP integration

---

## Core Rule (CRITICAL)

NEVER create new UI components if an equivalent exists.

---

## Design System Enforcement

- All UI must use shared components
- No hardcoded styles
- Tokens must be used

---

## Documentation First

Before generating code:
1. Check /docs
2. Check /libs/ui
3. Check existing usage

---

## Migration Strategy

- Strangler Fig Pattern
- Incremental replacement
- No big bang rewrite