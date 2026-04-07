# TrackVagas

> Transforme o caos de candidaturas em um Kanban organizado.
> Cole o texto do email ou faça upload de um print — o app extrai
> os dados automaticamente e você só confirma.

[Demo ao vivo →](link)

---

## O problema
Devs que enviam 50–100 candidaturas/mês perdem o controle: 
não lembram o cargo, salário, empresa, em qual etapa estão. 
Planilhas são pouco intuitivas.

## A solução
1. Cole o texto do email ou faça upload de um print
2. OCR + extração inteligente preenche os campos automaticamente
3. Você confirma em ~15 segundos
4. Candidatura vai direto para o Kanban

## Stack
**Backend:** Node.js · Express · MongoDB · tesseract.js · multer  
**Frontend:** React · Vite · TypeScript  
**Deploy:** Render · Vercel · MongoDB Atlas

## Status
- [x] Semana 1 — Backend base (Express + MongoDB + CRUD)
- [ ] Semana 2 — Ingestão inteligente (OCR + extração de campos)
- [ ] Semana 3 — Kanban com drag & drop
- [ ] Semana 4 — Score de fit + notas + export CSV

## Rodando localmente
```bash
git clone https://github.com/gabrifgaraujo/track-vagas
cd track-vagas/packages/backend
cp .env.example .env
npm install && npm run dev
```

## Limitações conhecidas (MVP)
- OCR pode levar 3–8s em imagens grandes no plano gratuito do Render
- Storage de imagens é temporário — não persistido entre deploys
