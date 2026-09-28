# Gamer Aesthetic — inventário de imagens do site

**Revisão:** 2026-09-28  
**Escopo:** assets necessários para homepage, catálogo, artigos, autora e distribuição social.

## Diagnóstico atual

Existem 5 imagens em `public/images/`, mas nenhuma está conectada ao JSX atual via `next/image`:

| Asset | Dimensão | Estado | Uso recomendado |
|---|---:|---|---|
| `hero/hero-main.png` | 1536×1024 | existente | hero da homepage; setup com monitor ultrawide, teclado e torre |
| `authors/tara-lindqvist.png` | 1024×1024 | existente | avatar/byline da autora e bloco editorial About |
| `articles/artigo-01-gaming-monitors.png` | 1536×1024 | existente | capa de monitores; adequada para o artigo de displays |
| `articles/artigo-02-wired-vs-wireless-headsets.png` | 1536×1024 | existente | capa de headsets; produto genérico sem marca visível |
| `articles/artigo-03-beginner-gaming-setup.png` | 1536×1024 | existente | capa de setup iniciante; composição ampla para card/hero |

## Assets criados nesta execução

As 7 capas que faltavam foram geradas e salvas em `articles/`:

- `gaming-compatibility-ps5-xbox-pc.png`
- `mechanical-keyboard-gaming-work.png`
- `1080p-vs-1440p-gaming.png`
- `clean-gaming-desk-small-rooms.png`
- `what-refresh-rate-means.png`
- `gaming-desk-ergonomics-basics.png`
- `gaming-setup-three-budgets.png`

Também foram criados:

- `brand/logo-gamer-aesthetic.svg`
- `brand/favicon.svg`
- `social/og-default.png`

Os 10 registros do catálogo agora têm `image` e `imageAlt`; homepage, cards, página de artigos e metadata Open Graph usam os assets correspondentes.
## Assets ainda opcionais

- `authors/tara-lindqvist-wide.png` — somente se o bloco About exigir composição horizontal.

## Critérios de produção

- Gerar PNG/WebP em 16:10 ou 3:2 para capas; manter uma área segura para crop no card.
- Exportar versão otimizada e registrar dimensões, alt text e origem em `public/images/README.md`.
- Não incluir logos de fabricantes, personagens licenciados, marcas registradas ou texto factual não verificado.
- Não inserir preço, FPS, Hz, resolução ou compatibilidade na arte; esses dados devem permanecer no HTML editorial revisável.
- Usar nomes sem acento e estáveis por slug.
- Após geração, conectar cada asset ao campo `image` do catálogo e renderizar com `next/image`.
- Verificar contraste, crop móvel, alt text e ausência de layout shift.

## Ordem recomendada

1. Criar as 7 capas de artigos faltantes;
2. Criar logo/favicon e OG default;
3. Adicionar `image`, `imageAlt` e dimensões ao contrato de conteúdo;
4. Implementar `next/image` nos cards, hero e template de artigo;
5. Atualizar metadata/Open Graph por artigo;
6. Rodar build e QA visual desktop/mobile.

## Decisão de uso

As imagens existentes são adequadas como primeira versão editorial, mas não devem ser tratadas como fotografia de produto real nem como prova de especificações. Elas funcionam como ilustração conceitual e devem receber alt text descritivo, sem claims técnicos.
