# Site do Innovatech

Site estático (HTML + CSS, sem build). Funciona direto no GitHub Pages.

## Antes de publicar

Edite só o **`config.js`**:

- `whatsapp` — número com DDI e DDD, só dígitos (ex.: `5517991234567`)
- `email` — e-mail de contato
- `download` — link do instalador
- `cnpj`, `cidade` — dados do rodapé
- `termos` — link dos Termos de Uso (vazio esconde o link)

**Link do instalador:** anexe o `Innovatech-Setup.exe` numa release do repositório
`innovatech-atualizacoes` e use o link direto:
`https://github.com/joaovitorbatistaaraujosilva/innovatech-atualizacoes/releases/latest/download/Innovatech-Setup.exe`

## Publicar no GitHub Pages

```
cd innovatech-site
git init
git add .
git commit -m "Site Innovatech"
git branch -M main
git remote add origin https://github.com/joaovitorbatistaaraujosilva/innovatech-site.git
git push -u origin main
```

No GitHub: **Settings > Pages > Source: Deploy from a branch > main / (root) > Save**.
Em 1 a 2 minutos o site fica em `https://joaovitorbatistaaraujosilva.github.io/innovatech-site/`.

## Domínio próprio (opcional)

1. Crie um arquivo `CNAME` com o domínio, por exemplo `www.innovatech.com.br`.
2. No DNS do domínio, crie um registro **CNAME** `www` apontando para `joaovitorbatistaaraujosilva.github.io`.
3. Em Settings > Pages, preencha o domínio e marque **Enforce HTTPS**.
