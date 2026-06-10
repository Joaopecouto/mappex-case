<h1 align="center">Mappex — Gerador de Leads</h1>

<p align="center">
  SaaS de geração de leads B2B com CRM integrado no WhatsApp.<br>
  <sub><i>B2B lead-generation SaaS with a built-in WhatsApp CRM.</i></sub>
</p>

<p align="center">
  <a href="https://gerador-de-leads.alcetus.com"><img src="https://img.shields.io/badge/Demo-gerador--de--leads.alcetus.com-1F4A7D?style=flat-square&logo=googlechrome&logoColor=white" alt="Demo"></a>
  <img src="https://img.shields.io/badge/source-private-555555?style=flat-square&logo=github&logoColor=white" alt="Source private">
</p>

> 📌 **Estudo de caso / Case study.** O código-fonte é privado; este repositório é a vitrine do projeto. · <i>Source code is private; this repo is the showcase.</i>

![Mappex](./screenshots/login.png)

---

## 🇧🇷 Português

### O problema
Pequenas empresas perdem horas procurando clientes manualmente e gerenciando conversas espalhadas no WhatsApp, sem processo nem acompanhamento.

### A solução
Plataforma que **encontra empresas por região**, **dispara campanhas** e centraliza o relacionamento num **CRM com WhatsApp** — do primeiro contato ao fechamento.

### Funcionalidades
- 🔎 Geração de leads por nicho + região via **Serper**, com **classificação de bairros por IA (Llama 3.3 / Groq)**
- 💬 **CRM com pipeline Kanban** e chat em tempo real (**Meta Cloud API / Evolution**)
- 🤖 Automações por gatilho (sem resposta em X horas, palavra-chave, etc.)
- 📧 Campanhas de e-mail (**Resend**) e fluxos de remarketing
- 🔐 Autenticação JWT + Google OAuth, rate-limiting e detecção de incidentes de segurança

### Stack & arquitetura
- **Front-end:** React 19, TypeScript, Vite, Tailwind CSS
- **Back-end:** NestJS + Fastify, Drizzle ORM, PostgreSQL, filas com pg-boss
- **Evolução de arquitetura:** v1 em **Supabase / Edge Functions (Deno)** → **backend próprio em NestJS**
- **Infra:** Docker, Nginx, VPS, Cloudflare
- **Escala:** 28 tabelas no banco · 8+ integrações externas

---

## 🇺🇸 English

**The problem.** Small businesses waste hours prospecting by hand and juggling scattered WhatsApp chats with no process.

**The solution.** A platform that **finds companies by region**, **runs campaigns** and centralizes everything in a **WhatsApp CRM** — from first contact to close.

**Highlights**
- 🔎 Lead generation by niche + region via **Serper**, with **AI neighborhood ranking (Llama 3.3 / Groq)**
- 💬 **Kanban CRM** with real-time WhatsApp chat (**Meta Cloud API / Evolution**)
- 🤖 Trigger-based automations · 📧 email campaigns (**Resend**) + remarketing
- 🔐 JWT + Google OAuth, rate-limiting, security-incident detection

**Stack:** React 19 · TypeScript · NestJS + Fastify · Drizzle · PostgreSQL · Docker · Nginx — re-architected from Supabase/Edge Functions to a dedicated NestJS backend. 28 tables, 8+ integrations.

---

<sub>🖼️ Mais telas (dashboard, gerador, CRM Kanban, chat) em breve. · More screens coming soon.</sub>
