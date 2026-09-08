# Site — Escritório de Advocacia (Bootstrap 5.3)

Site estático usando Bootstrap 5.3 via CDN + um CSS de customização. Sem build, sem npm: basta hospedar os arquivos.

## Estrutura

```
advocacia-bs/
├── index.html       → página inicial (hero, áreas, sobre, prévia do blog, contato)
├── blog.html        → listagem de artigos
├── artigo.html      → modelo de artigo (duplique para cada post)
└── css/custom.css   → identidade visual sobre o Bootstrap
```

O JS do Bootstrap (bundle, via CDN) já cuida do menu mobile (navbar collapse) — não há JS próprio.

## O que personalizar

1. **Nome e dados** — busque por "Advocacia" e substitua (nome, OAB, endereço, telefone, e-mail).
2. **WhatsApp** — troque `5585999990000` nos links `wa.me`.
3. **Formulário** — troque `SEU_ID_AQUI` na action (Formspree) ou aponte para um Google Apps Script (doPost gravando numa planilha).
4. **Cores/fontes** — variáveis `--vp-*` no topo de `css/custom.css`. As variáveis do Bootstrap (`--bs-body-bg`, `--bs-link-color` etc.) já estão sobrescritas lá.

## Componentes Bootstrap usados

- `navbar` + `collapse` (menu responsivo)
- Grid (`row`/`col-*`) em todas as seções
- `card` nos posts da home
- `form-control`, `form-select`, `form-label` no contato
- `badge` nas tags do blog
- Botões customizados via variáveis CSS do Bootstrap (`.btn-vp`, `.btn-vp-outline`)

## Novo artigo

1. Duplique `artigo.html` com um nome descritivo.
2. Edite título, meta description, data e conteúdo.
3. Adicione o item correspondente em `blog.html` (e opcionalmente um card na home).

## Hospedagem gratuita

GitHub Pages, Netlify, Vercel ou Cloudflare Pages — é só enviar a pasta.

## Observação ética (OAB)

O Provimento 205/2021 permite sites e marketing de conteúdo informativo, sem
mercantilização nem promessa de resultado. O rodapé já traz o aviso — mantenha-o.
