# AIFLUENT Website

Site institucional estático e responsivo da AIFLUENT ("Infrastructure for High-Performance Education Companies"), com design inspirado nos padrões da Apple. Versões em inglês e português.

## Stack

- **Linguagem**: HTML5, CSS3 e JavaScript vanilla — **sem framework e sem build step**.
- **Estilo**: um único stylesheet em `assets/css/style.css`; fonte Inter carregada via Google Fonts.
- **JS**: `assets/js/script.js` (interações de navegação/UI).
- **Banco/backend**: nenhum. É 100% front-end estático.
- **Package manager**: nenhum (não há `package.json` nem dependências npm).
- **Deploy**: hospedagem estática (serve os `.html` da raiz). Não há `vercel.json`/`netlify.toml` versionado.

## Comandos

Não há scripts de build/test/lint — o projeto é estático. Para desenvolver localmente, sirva a pasta com qualquer servidor estático, por exemplo:

```bash
python3 -m http.server 8000      # abre em http://localhost:8000
# ou
npx serve .
```

Abrir os `.html` direto no navegador (`file://`) também funciona para a maior parte, mas um servidor local evita problemas de caminho/CORS.

## Estrutura

```
index.html         # homepage (EN)
pt.html            # homepage (PT)
solutions.html     # página de soluções (EN)
solucoes.html      # página de soluções (PT)
assets/css/style.css   # stylesheet único (cores de marca, layout, responsivo)
assets/js/script.js    # JS de interação
assets/images/         # logo e imagens (ver "Image Requirements" no README)
README.md          # documentação de marca, cores e assets esperados
```

## Convenções de código

- HTML semântico e acessível (o README enfatiza acessibilidade e SEO).
- **Paridade EN/PT**: qualquer mudança de conteúdo/estrutura deve ser replicada nos pares `index.html`↔`pt.html` e `solutions.html`↔`solucoes.html`.
- **Cores de marca** (do README) — usar sempre estas: Primary Blue `#1A3C5A`, Secondary Blue `#546A76`, Accent Gold `#B89B5E`, Cream `#F4F0E3`, White `#FFFFFF`.
- CSS centralizado em `style.css`; evitar estilos inline dispersos.
- Manter dependências externas mínimas (só a fonte via CDN) para carregamento rápido.

## Variáveis de ambiente

Nenhuma — site estático, sem segredos e sem configuração de runtime.

## CI/CD & Deploy

- **Hoje**: sem GitHub Actions e sem config de deploy versionada.
- **Recomendado (mínimo, opcional)**: um workflow leve em PR rodando um **HTML/link validator** (ex.: `html-validate` ou lychee para checar links quebrados) e conferindo que os pares EN/PT existem. Para um site estático não é necessário pipeline de build/lint pesado.

## Boas práticas de PR

- Branch naming: `feat/…`, `fix/…`, `chore/…`.
- **Conventional Commits** (`feat:`, `fix:`, `docs:`, `style:`…).
- PRs pequenos e focados; **inclua screenshots** (desktop e mobile) de qualquer alteração visual, já que não há testes.
- Checklist: páginas abrem sem erro de console, layout responsivo mantido, paridade EN/PT preservada, nenhum segredo commitado.
- ≥1 review, **squash merge**, manter a `main` sempre publicável.

## Testes

Não há testes automatizados e, para um site institucional estático, não são necessários. Verificação manual: abrir cada página em desktop e mobile, checar navegação, links e responsividade.

## Segurança & dados

- Não há dados pessoais nem segredos — mantenha assim (nada de `.env`, chaves ou tokens no repo).
- Ao adicionar scripts de terceiros (analytics, formulários), prefira carregamento com `defer`/`async` e revise a origem.
- Imagens/assets: otimize antes de commitar para não inflar o repositório.

## Gotchas

- **Quatro páginas espelhadas (EN/PT)** — o erro mais comum é editar só uma língua. Sempre atualize o par correspondente.
- O README lista imagens esperadas em `assets/images/` que podem ainda não existir (ex.: `aifluent-logo.svg`, imagens de hero). Confirme os caminhos antes de referenciar assets no HTML.
- Sem build: o que está no repo é exatamente o que vai para produção — não há transpile/minify. Escreva HTML/CSS/JS já prontos para produção.
- A fonte Inter vem de CDN (Google Fonts): sem internet ela cai no fallback do sistema.
