# CLAUDE.md — PONTOCOMM

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** PONTOCOMM
**Nicho:** Educação
**Keywords:** Pontocomm e uma agencia de comunicacao e marketing que nasceu da uniao
**Paleta de cores:** slate | **Fonte:** poppins

Pontocomm é uma agência de comunicação e marketing que nasceu da união de três amigos apaixonados por ideias inovadoras. Juntos, somam mais de 20 anos de experiência no mercado publicitário. Sempre em busca de soluções criativas e ousadas, a Pontocomm se destaca pela capacidade de traduzir os desejos dos clientes em campanhas bem-sucedidas. Com um time multidisciplinar, a agência atua na concepção de campanhas para expandir o alcance e consequentemente as vendas dos nossos clientes.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-I |
| Hero | Hero-E |
| Features | Features-D |
| About Section | About-G |
| Posts | Posts-G |
| Footer | Footer-J |
| Página Sobre | Sobre-C |
| Página Contato | Contato-E |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
