# ShopReply — Cold Email Generator

Mini SaaS de génération de cold emails pour ShopReply.

## Stack
- Frontend : HTML/CSS/JS vanilla
- Backend : Vercel Serverless Functions (proxy API)
- LLM : GPT-4o
- Data : Notion API

## Déploiement sur Vercel

### Méthode 1 — GitHub (recommandée)
1. Push ce dossier sur GitHub
2. Va sur vercel.com → New Project → Importe ton repo
3. Vercel détecte automatiquement la config
4. Deploy !

### Méthode 2 — CLI
```bash
npm install -g vercel
vercel
```

## Structure
```
shopreply-saas/
├── api/
│   ├── notion/[...path].js   # Proxy Notion API
│   ├── openai.js             # Proxy OpenAI API
│   └── fetch-site.js         # Fetch contenu des sites
├── public/
│   └── index.html            # Frontend
├── vercel.json               # Config Vercel
└── package.json
```

## Utilisation
1. Ouvre l'URL Vercel dans ton navigateur
2. Entre ta clé OpenAI + token Notion (sauvegardés localement)
3. Charge les prospects depuis ta base Notion "Prospect"
4. Lance la génération
5. Clique "Gmail →" pour envoyer chaque email
