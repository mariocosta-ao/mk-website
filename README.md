# MUKANDA — Website Institucional

> **"Tecnologia que cresce contigo."**  
> Guiados pela filosofia Ubuntu — *"Sou porque somos"* — construímos soluções digitais com propósito, alma e identidade africana.

---

## 📋 Índice

1. [Visão geral do projeto](#-visão-geral-do-projeto)
2. [Demonstração](#-demonstração)
3. [Tecnologias utilizadas](#-tecnologias-utilizadas)
4. [Estrutura de pastas](#-estrutura-de-pastas)
5. [Como começar](#-como-começar)
6. [Páginas e secções](#-páginas-e-secções)
7. [Identidade visual](#-identidade-visual)
8. [Scripts e funcionalidades JS](#-scripts-e-funcionalidades-js)
9. [Responsividade](#-responsividade)
10. [Personalização de conteúdo](#-personalização-de-conteúdo)
11. [Deploy e publicação](#-deploy-e-publicação)
12. [Roadmap](#-roadmap)
13. [Equipa](#-equipa)
14. [Licença](#-licença)

---

## 🌍 Visão geral do projeto

O **MUKANDA Website** é o site institucional oficial da empresa MUKANDA, uma empresa angolana de tecnologia com sede em Luanda. O site foi desenvolvido com foco em:

- ✅ **Alta conversão** — CTAs estratégicos em múltiplas secções
- ✅ **Identidade de marca forte** — cores, tipografia e tom de voz consistentes
- ✅ **Filosofia Ubuntu** — "crescemos juntos" como fio condutor
- ✅ **Mercado angolano** — conteúdo e contexto adaptados ao negócio local
- ✅ **Performance** — HTML/CSS/JS puro, sem dependências pesadas
- ✅ **Totalmente responsivo** — mobile, tablet e desktop

### Serviços apresentados
| # | Serviço |
|---|---|
| 1 | Desenvolvimento Web & Sistemas |
| 2 | Design Gráfico & Branding |
| 3 | Gestão de Redes Sociais |
| 4 | Infraestrutura & Redes |
| 5 | CCTV & Segurança |
| 6 | Suporte Técnico |

---

## 🖥️ Demonstração

> 🔗 **URL de produção:** `https://www.mukanda.ao` *(após deploy)*  
> 🔗 **Preview de staging:** *(configurar via Netlify)*

**Screenshot — Hero Section:**
```
┌─────────────────────────────────────────────┐
│  MUKANDA                    [Falar Connosco] │
├─────────────────────────────────────────────┤
│                                             │
│  A tecnologia certa                         │
│  para crescer junto                         │
│  ao seu negócio.          [Fundo escuro     │
│                            com orbs         │
│  [Ver Serviços] [Projetos]  animados]       │
│                                             │
│  +50 Projetos  |  +30 Clientes  |  6 Áreas │
└─────────────────────────────────────────────┘
```

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Versão | Função |
|---|---|---|
| HTML5 | — | Estrutura semântica |
| CSS3 | — | Estilos, animações, layout (Grid + Flexbox) |
| JavaScript | ES6+ | Interactividade, animações, formulário |
| Google Fonts | — | Ubuntu + Lato (via CDN) |

### Dependências externas
```html
<!-- Única dependência externa: Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Ubuntu:wght@300;400;500;700&family=Lato:wght@300;400;700;900&display=swap" rel="stylesheet">
```

**Zero frameworks. Zero bibliotecas JS. Zero dependências npm.**  
O site funciona abrindo `index.html` directamente no browser.

---

## 📁 Estrutura de pastas

```
mukanda-website/
│
├── 📄 README.md                     ← Este ficheiro
├── 📄 CHANGELOG.md                  ← Histórico de versões
├── 📄 CONTRIBUTING.md               ← Guia de contribuição
├── 📄 .gitignore                    ← Ficheiros ignorados pelo Git
│
├── 📁 src/                          ← Código fonte do website
│   │
│   ├── 📄 index.html                ← Página principal (SPA com todas as secções)
│   │
│   ├── 📁 assets/
│   │   │
│   │   ├── 📁 css/
│   │   │   └── 📄 styles.css        ← Folha de estilos principal
│   │   │
│   │   ├── 📁 js/
│   │   │   └── 📄 main.js           ← Script principal
│   │   │
│   │   ├── 📁 img/
│   │   │   ├── 📁 hero/             ← Imagens da secção hero
│   │   │   ├── 📁 portfolio/        ← Thumbnails dos projetos
│   │   │   ├── 📁 team/             ← Fotografias da equipa
│   │   │   ├── 📁 blog/             ← Imagens de capa dos artigos
│   │   │   └── 📁 logo/             ← Logótipos, favicon, OG image
│   │   │
│   │   ├── 📁 fonts/                ← Fontes locais (fallback, se necessário)
│   │   └── 📁 icons/                ← Ícones SVG personalizados
│   │
│   ├── 📁 components/               ← Fragmentos HTML reutilizáveis (expansão futura)
│   └── 📁 pages/                    ← Páginas HTML adicionais (expansão futura)
│
└── 📁 docs/
    ├── 📄 STYLE_GUIDE.md            ← Guia de estilo (cores, tipografia, componentes)
    └── 📄 DEPLOY.md                 ← Instruções de deploy e manutenção
```

---

## 🚀 Como começar

### Pré-requisitos
- Qualquer browser moderno (Chrome, Firefox, Safari, Edge)
- Editor de código: [VS Code](https://code.visualstudio.com/) (recomendado)
- Extensão VS Code: [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (para desenvolvimento com hot reload)

### Instalação e execução local

```bash
# 1. Clonar o repositório
git clone https://github.com/mukanda/website.git

# 2. Entrar na pasta do projeto
cd mukanda-website

# 3. Abrir no VS Code
code .

# 4. Iniciar com Live Server
# → Clique com o botão direito em src/index.html
# → "Open with Live Server"
# → O site abre em http://127.0.0.1:5500/src/
```

**Ou simplesmente:**
```bash
# Abrir directamente no browser (sem servidor)
open src/index.html         # macOS
start src/index.html        # Windows
xdg-open src/index.html     # Linux
```

> ⚠️ **Nota:** As fontes do Google Fonts requerem ligação à internet.  
> Para uso offline, copie os ficheiros de fonte para `src/assets/fonts/` e actualize o CSS.

---

## 📑 Páginas e secções

O site é uma **Single Page Application (SPA)** — todas as secções estão em `index.html` e a navegação é feita por âncoras com scroll suave.

| Âncora | Secção | Descrição |
|---|---|---|
| `#home` | Hero | Headline principal, estatísticas, CTAs |
| — | Benefícios | 6 cards com os principais diferenciais |
| `#servicos-home` | Serviços (resumo) | Preview dos 6 serviços com links |
| — | Filosofia Ubuntu | Citação e valores da empresa |
| — | CTA Banner | Chamada para acção de conversão |
| `#sobre` | Sobre nós | História, missão, visão, valores |
| `#servicos` | Serviços completos | Descrição detalhada dos 6 serviços |
| `#projetos` | Portfólio | 6 projetos com filtros por categoria |
| `#equipa` | Equipa | 6 membros + cultura da empresa |
| `#blog` | Blog | 6 artigos de conteúdo educativo |
| `#faq` | FAQ | 10 perguntas em 4 categorias |
| `#contacto` | Contacto | Formulário + info + WhatsApp CTA |
| — | Footer | Links, redes sociais, tagline |

---

## 🎨 Identidade visual

### Paleta de cores

```css
--blue:       #0049FF;   /* Azul principal — CTAs, links, destaque */
--blue-dark:  #001B5E;   /* Azul escuro — fundos, textos fortes */
--orange:     #F25623;   /* Laranja — accent, hover, badges */
--gray:       #DEDEDE;   /* Cinza — bordas, separadores */
--bg-dark:    #040D2B;   /* Fundo escuro (secções de contraste) */
--bg-light:   #F7F8FC;   /* Fundo claro (secções alternadas) */
```

### Tipografia

```css
--font-title: 'Ubuntu', sans-serif;   /* Títulos, headings, logo, botões */
--font-body:  'Lato', sans-serif;     /* Corpo de texto, parágrafos, labels */
```

### Consultar documentação completa
→ [`docs/STYLE_GUIDE.md`](docs/STYLE_GUIDE.md)

---

## ⚙️ Scripts e funcionalidades JS

Todas as funcionalidades estão em `src/assets/js/main.js` sem dependências externas.

| Funcionalidade | Descrição |
|---|---|
| **Navbar scroll** | Adiciona fundo escuro + blur ao scroll |
| **Menu mobile** | Hamburger com overlay fullscreen |
| **Scroll suave** | Navegação com offset para a navbar fixa |
| **Fade-in ao scroll** | Intersection Observer com `translateY` |
| **Contador de stats** | Animação numérica nas estatísticas do hero |
| **FAQ acordeão** | Abre/fecha perguntas com transição CSS |
| **Filtros de portfólio** | Filtragem por categoria com fade |
| **Formulário de contacto** | Validação + feedback visual de sucesso |
| **Nav link activo** | Destaca o link da secção visível no scroll |
| **Botão voltar ao topo** | Aparece ao scroll, scroll suave ao topo |

---

## 📱 Responsividade

O site foi construído com uma abordagem **desktop-first com adaptação completa** para todos os tamanhos de ecrã.

| Breakpoint | Largura | Comportamento principal |
|---|---|---|
| Desktop | > 1024px | Layout completo, grids de 3 colunas |
| Tablet | ≤ 1024px | Grids 2 colunas, layouts ajustados |
| Mobile | ≤ 768px | Stack vertical, 1 coluna, menu hamburger |

**Testado em:**
- ✅ iPhone SE (375px)
- ✅ iPhone 14 (390px)
- ✅ Samsung Galaxy S21 (360px)
- ✅ iPad (768px)
- ✅ iPad Pro (1024px)
- ✅ Desktop (1280px, 1440px, 1920px)

---

## ✏️ Personalização de conteúdo

### 1. Dados de contacto
Pesquisar e substituir em `src/index.html`:

```
+244 9XX XXX XXX    → número de telefone real
geral@mukanda.ao    → email real
suporte@mukanda.ao  → email de suporte real
```

### 2. Redes sociais
Localizar os links `<a href="#">` na secção de contacto e footer e substituir pelos URLs reais:
```html
<!-- Exemplo -->
<a href="https://www.linkedin.com/company/mukanda" class="social-btn">in</a>
<a href="https://www.facebook.com/mukanda.ao" class="social-btn">f</a>
<a href="https://www.instagram.com/mukanda.ao" class="social-btn">ig</a>
```

### 3. WhatsApp
Substituir o link do botão WhatsApp pelo número real:
```html
<a href="https://wa.me/244XXXXXXXXX?text=Olá%2C%20gostaria%20de%20mais%20informações"
   class="btn-whatsapp">
```

### 4. Imagens
Adicionar imagens reais nas pastas correspondentes e referenciar no HTML:
```html
<!-- Exemplo: substituir emoji por imagem real -->
<img src="assets/img/portfolio/portfolio-clinica-medcare-thumb.webp"
     alt="Projeto Clínica MedCare Luanda">
```

### 5. Formulário de contacto
O formulário usa um handler JavaScript de demonstração. Para receber emails reais, integrar com:

**Opção A — Formspree (gratuito, sem backend):**
```html
<form action="https://formspree.io/f/SEU_ID" method="POST">
```

**Opção B — EmailJS (gratuito até 200 emails/mês):**
```javascript
// Em main.js, substituir o setTimeout por:
emailjs.send('SERVICE_ID', 'TEMPLATE_ID', formData);
```

**Opção C — Backend próprio (PHP/Node.js):**
```html
<form action="/api/contacto" method="POST">
```

---

## 🚢 Deploy e publicação

Consultar o guia completo em [`docs/DEPLOY.md`](docs/DEPLOY.md).

**Resumo rápido — Netlify (recomendado):**
```bash
# Arrastar a pasta src/ para app.netlify.com
# OU usar Netlify CLI:
npm install -g netlify-cli
netlify deploy --dir=src --prod
```

**Checklist pré-lançamento:**
- [ ] Substituir todos os dados de contacto placeholder
- [ ] Adicionar imagens reais
- [ ] Configurar formulário de contacto
- [ ] Adicionar favicon e OG image
- [ ] Configurar domínio `mukanda.ao`
- [ ] Activar HTTPS/SSL
- [ ] Instalar Google Analytics

---

## 🗺️ Roadmap

### v1.0.0 — Lançamento ✅
- Website institucional completo (SPA)
- Todas as secções e páginas
- Design responsivo
- Funcionalidades JS

### v1.1.0 — Planeado
- [ ] Integração de formulário (Formspree / EmailJS)
- [ ] Favicon e OG Image reais
- [ ] Imagens reais de equipa e portfólio
- [ ] Google Analytics 4
- [ ] Meta Pixel
- [ ] Open Graph / SEO tags completas

### v1.2.0 — Futuro
- [ ] Blog dinâmico (integração com CMS: Sanity, Contentful ou Strapi)
- [ ] Página 404 personalizada
- [ ] Política de Privacidade
- [ ] Animações avançadas (GSAP ScrollTrigger)
- [ ] Modo escuro / claro (toggle)
- [ ] Chat ao vivo (WhatsApp Business Widget)

### v2.0.0 — Visão
- [ ] Migração para framework (Next.js ou Astro)
- [ ] Área de cliente com login
- [ ] Portal de pedidos e suporte
- [ ] Dashboard de acompanhamento de projetos

---

## 👥 Equipa

| Nome | Papel no projeto |
|---|---|
| Kizua Mendes | CEO, direcção estratégica |
| Ana Lima | Direcção criativa e design |
| Jonas Neto | Desenvolvimento frontend |
| Sofia Francisco | Estratégia de conteúdo |

---

## 📄 Licença

**Proprietário — Todos os direitos reservados.**

```
Copyright © 2025 MUKANDA — Todos os direitos reservados.

Este código e todos os activos associados são propriedade exclusiva da MUKANDA.
É proibida a reprodução, distribuição ou modificação sem autorização expressa
por escrito da MUKANDA.

Para licenciamento ou parcerias: geral@mukanda.ao
```

---

## 📞 Contacto do projeto

| Canal | Info |
|---|---|
| 🌐 Website | https://www.mukanda.ao |
| ✉️ Email | geral@mukanda.ao |
| 📞 Telefone | +244 9XX XXX XXX |
| 💬 WhatsApp | +244 9XX XXX XXX |
| 📍 Localização | Luanda, Angola |

---

<div align="center">

**Feito com 🧡 em Luanda, Angola**

*Ubuntu — "Sou porque somos"*

</div>
