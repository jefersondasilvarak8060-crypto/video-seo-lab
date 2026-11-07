# Video SEO Lab — Cloudflare Pages

Teste inicial de hospedagem estática. Site de teste, **não indexar**.

## Estrutura

- `index.html`: página inicial do laboratório.
- `videos/horse-gelatin-trick/index.html`: página com player VTurb e CTA.
- `video-sitemap.xml`: XML válido, vazio **de propósito** nesta fase.
- `_headers`: cabeçalho `X-Robots-Tag: noindex, nofollow` para todas as rotas.

## Deploy com Cloudflare Pages

1. No painel Cloudflare, crie o projeto Pages integrado a este repositório.
2. Branch de produção: `main`.
3. Framework: `None`; build command: deixe vazio; output directory: `/` (raiz do projeto), conforme o campo do painel.
4. Após o deploy, abra a home, `/videos/horse-gelatin-trick/` e `/video-sitemap.xml`.
5. Verifique HTTP 200, vídeo e botão, e confirme que o XML é servido como XML.

**Não envie essas URLs ao Search Console:** o vídeo é um teste técnico de duplicação da página já publicada no domínio Atomicat. O sitemap está vazio. A versão real precisa de vídeo/página originais e URL canônica definitiva, antes de remover `noindex`.

O conteúdo da página é destinado a visitantes dos EUA e está em inglês. README técnico mantido em português.
