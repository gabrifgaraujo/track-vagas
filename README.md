# AutoVagas

> Agregador automático de vagas de TI — busca, processa e ranqueia 
> vagas do LinkedIn e Gupy com base no seu perfil. Zero trabalho manual.

[Demo](link) · [API Docs](link) · [Report Bug](issues)

---

## Como funciona

1. Você configura seu perfil de busca uma vez
2. O sistema busca vagas 4x por dia automaticamente  
3. Vagas são processadas, deduplicadas e ranqueadas por fit
4. Você recebe alertas apenas das vagas que combinam com você

## Stack

**Backend:** Node.js · Express · MongoDB · node-cron  
**Frontend:** React · Vite · TypeScript  
**Deploy:** Render (API) · Vercel (Frontend) · MongoDB Atlas

## Rodando localmente
```bash
git clone https://github.com/gabrifgaraujo/autovagas
cd autovagas/packages/backend
cp .env.example .env   # configure suas variáveis
npm install
npm run dev
```

## Variáveis de ambiente

| Variável | Descrição |
|---|---|
| `MONGODB_URI` | Connection string do MongoDB Atlas |
| `JWT_SECRET` | Secret para assinar os tokens |
| `TELEGRAM_BOT_TOKEN` | Token do bot de alertas |

## Status do projeto

- [ ] Semana 1 — Backend base (Express + MongoDB + Auth)
- [ ] Semana 2 — Scraping LinkedIn e Gupy
- [ ] Semana 3 — Pipeline de processamento
- [ ] Semana 4 — Dashboard React + Deploy
