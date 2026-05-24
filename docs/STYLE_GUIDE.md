# Guia de Estilo — MUKANDA

Documento de referência para manter consistência visual e de código em todo o projeto.

---

## 🎨 Identidade Visual

### Paleta de Cores

| Nome | Hex | Uso |
|---|---|---|
| Azul Principal | `#0049FF` | CTAs, links, destaques, bordas activas |
| Azul Escuro | `#001B5E` | Fundo escuro, títulos sobre fundo claro |
| Laranja | `#F25623` | Accent, hover states, badges, números |
| Cinza | `#DEDEDE` | Bordas, separadores, fundos subtis |
| Branco | `#FFFFFF` | Fundo principal, texto sobre escuro |
| Preto suave | `#0A0A0A` | Texto principal |
| Fundo escuro | `#040D2B` | Secções de contraste alto |
| Fundo claro | `#F7F8FC` | Secções alternadas de fundo claro |
| Texto | `#1A1A2E` | Corpo de texto principal |
| Texto suave | `#5A5A7A` | Texto secundário, descrições |

### CSS Variables
```css
:root {
  --blue:       #0049FF;
  --blue-dark:  #001B5E;
  --orange:     #F25623;
  --gray:       #DEDEDE;
  --white:      #FFFFFF;
  --black:      #0A0A0A;
  --text:       #1A1A2E;
  --text-light: #5A5A7A;
  --bg-light:   #F7F8FC;
  --bg-dark:    #040D2B;
}
```

---

## ✍️ Tipografia

### Fontes
| Função | Fonte | Pesos |
|---|---|---|
| Títulos, headings, logo | **Ubuntu** | 300, 400, 500, 700 |
| Corpo, botões, labels | **Lato** | 300, 400, 700, 900 |

### Hierarquia tipográfica
```
H1  — clamp(2.4rem, 6vw, 4.2rem) — Ubuntu 700 — Hero
H2  — clamp(2rem, 4vw, 2.8rem)   — Ubuntu 700 — Títulos de secção
H3  — 1.1rem – 1.4rem            — Ubuntu 700 — Subtítulos, cards
H4  — 0.95rem                    — Ubuntu 700 — Rótulos, categorias
P   — 0.9rem – 1.15rem           — Lato 400    — Corpo de texto
```

---

## 🔘 Componentes UI

### Botões
```
.btn-primary    — Azul sólido, texto branco — acção principal
.btn-outline    — Borda branca, fundo transparente — sobre fundos escuros
.btn-outline-dark — Borda azul, texto azul — sobre fundos claros
.btn-white      — Fundo branco, texto escuro — sobre banners coloridos
.btn-nav        — Versão compacta para navbar
```

### Labels de secção
```css
/* Sempre usar .section-label antes do título da secção */
.section-label      — Fundo azul claro, texto azul — fundo claro
.section-label.light — Fundo branco translúcido — fundo escuro
```

### Cards
- **Border-radius:** `16px` (padrão), `8px` (pequeno)
- **Padding:** `28px – 40px`
- **Hover:** `translateY(-4px)` + `box-shadow`
- **Transição:** `0.3s cubic-bezier(.4,0,.2,1)`

---

## 📐 Espaçamento e Layout

### Container
- **Max-width:** `1200px`
- **Padding horizontal:** `24px`

### Secções
- **Padding vertical:** `100px 0` (desktop) / `72px 0` (mobile)

### Grid principal
- Benefícios: 3 colunas → 2 → 1
- Serviços: 3 colunas → 2 → 1
- Portfólio: 3 colunas → 2 → 1
- Equipa: 3 colunas → 2 → 1
- Blog: 2 colunas (featured + lateral) → 1
- FAQ: 2 colunas → 1
- Contacto: 2 colunas → 1

### Breakpoints
| Nome | Valor | Comportamento |
|---|---|---|
| Desktop | > 1024px | Layout completo |
| Tablet | ≤ 1024px | Grids reduzidos, 2 colunas |
| Mobile | ≤ 768px | Stack vertical, 1 coluna |

---

## 🖼️ Imagens

### Nomenclatura
```
[secção]-[descrição]-[variante].[ext]

hero-background-main.webp
portfolio-clinica-medcare-thumb.webp
team-kizua-mendes-photo.webp
blog-digitalizacao-angola-cover.webp
logo-mukanda-principal.svg
logo-mukanda-branco.svg
logo-mukanda-favicon.png
```

### Formatos e tamanhos recomendados
| Tipo | Formato | Tamanho máx. |
|---|---|---|
| Fotografias | WebP (fallback JPG) | 200KB |
| Logótipos | SVG | — |
| Ícones | SVG | — |
| Favicon | PNG 32×32 + ICO | 10KB |
| OG Image | JPG 1200×630 | 150KB |

---

## 🌍 Tom de comunicação

- **Directo e humano** — falar para pessoas, não para empresas
- **Confiante sem ser arrogante** — mostrar autoridade com humildade
- **Benefícios antes de features** — "poupa tempo" antes de "automação de processos"
- **Contexto angolano** — referências ao mercado local, não genéricas
- **Ubuntu como fio condutor** — crescimento partilhado em todas as mensagens
