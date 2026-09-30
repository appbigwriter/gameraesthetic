# Gamer Aesthetic — inventário de imagens

**Revisão:** 2026-09-29  
**Regra:** imagens realistas, sem SVG editorial.

## Assets publicados

Todos os assets atuais são fotografias realistas convertidas para WebP:

- `hero/hero-main.webp` — 1920×1080, hero da homepage
- `authors/tara-lindqvist.webp` — 600×600, avatar editorial
- `social/og-default.webp` — 1920×1080, Open Graph padrão
- 10 capas dedicadas em `articles/*.webp` — 1200×675

Capas: `gaming-monitors-by-setup`, `wired-vs-wireless-gaming-headsets`, `gaming-compatibility-ps5-xbox-pc`, `mechanical-keyboard-gaming-work`, `1080p-vs-1440p-gaming`, `clean-gaming-desk-small-rooms`, `what-refresh-rate-means`, `gaming-desk-ergonomics-basics`, `gaming-setup-three-budgets` e `gaming-setup-essentials-for-beginners`.

## Verificação

- 10/10 artigos possuem capa WebP dedicada.
- Hero, avatar e OG estão em WebP.
- Nenhum arquivo SVG permanece em `public/images`.
- Os caminhos são renderizados com `next/image`.
- Build de produção validado com 21 rotas geradas.

## Regras editoriais

- Não inserir preços, FPS, Hz, resolução, compatibilidade, logos ou texto factual dentro da imagem.
- Manter alt text descritivo e honesto, sem transformar fotografia em prova de especificação.
- Verificar crop móvel, contraste, peso e ausência de layout shift.

