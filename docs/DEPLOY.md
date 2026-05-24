# Guia de Deploy — MUKANDA Website

Instruções para publicação e manutenção do website em produção.

---

## 🚀 Opções de hospedagem recomendadas

### Opção A — Hosting partilhado (Angola / África)
Indicado para: lançamento rápido, orçamento limitado.

**Providers recomendados:**
- Angola Telecom / NetOne (hosting local)
- Afrihost (África do Sul, boa latência)
- Hostinger (internacional, boa relação custo/benefício)

**Passos:**
1. Fazer upload de todo o conteúdo da pasta `src/` via FTP/FileZilla
2. Garantir que `index.html` está na raiz pública (`public_html/` ou `www/`)
3. Configurar domínio `mukanda.ao` a apontar para os nameservers do hosting

### Opção B — GitHub Pages (gratuito)
Indicado para: demonstrações, testes, portfolio.

```bash
# 1. Criar repositório no GitHub
git init
git add .
git commit -m "feat: initial release v1.0.0"
git remote add origin https://github.com/mukanda/website.git
git push -u origin main

# 2. Activar GitHub Pages
# GitHub → Settings → Pages → Source: main / pasta src/
```

### Opção C — Netlify (recomendado para produção)
Indicado para: deploys automáticos, HTTPS gratuito, CDN global.

```bash
# 1. Instalar Netlify CLI (opcional)
npm install -g netlify-cli

# 2. Deploy manual
netlify deploy --dir=src --prod

# OU arrastar a pasta src/ para app.netlify.com
```

**Vantagens:** HTTPS automático, CDN, previews por branch, formulários nativos.

---

## 🌐 Configuração de domínio

### Domínio `.ao`
- Registo via: **NIC.ao** (https://nic.ao)
- Documentação exigida: NIF da empresa + documentos comerciais
- Prazo de registo: 5–10 dias úteis

### DNS Records típicos
```
Tipo    Nome    Valor
A       @       IP_DO_SERVIDOR
A       www     IP_DO_SERVIDOR
CNAME   www     mukanda.ao
MX      @       mail.mukanda.ao
```

---

## 🔒 HTTPS / SSL

- **Netlify / GitHub Pages:** SSL automático e gratuito (Let's Encrypt)
- **Hosting partilhado:** Activar SSL no painel de controlo (cPanel → SSL/TLS)
- Verificar que todos os links internos usam `https://`

---

## ✅ Checklist pré-lançamento

### Conteúdo
- [ ] Substituir todos os placeholders (`+244 9XX XXX XXX`, `geral@mukanda.ao`) por dados reais
- [ ] Adicionar imagens reais nas pastas `src/assets/img/`
- [ ] Rever todos os textos com o cliente
- [ ] Confirmar links de redes sociais

### Técnico
- [ ] Testar formulário de contacto (configurar destino do email)
- [ ] Verificar em Chrome, Firefox, Safari e Edge
- [ ] Verificar em dispositivos iOS e Android
- [ ] Validar HTML: https://validator.w3.org
- [ ] Validar CSS: https://jigsaw.w3.org/css-validator
- [ ] Testar velocidade: https://pagespeed.web.dev

### SEO
- [ ] Preencher `<title>` e `<meta name="description">` em cada página
- [ ] Adicionar Open Graph tags (`og:title`, `og:image`, `og:description`)
- [ ] Criar `sitemap.xml`
- [ ] Criar `robots.txt`
- [ ] Adicionar favicon (`/src/assets/img/logo/favicon.ico`)
- [ ] Registar no Google Search Console

### Analytics
- [ ] Instalar Google Analytics 4 (tag no `<head>`)
- [ ] Instalar Meta Pixel (se usar publicidade no Facebook/Instagram)
- [ ] Configurar eventos de conversão (clique no CTA, envio de formulário)

---

## 🔧 Manutenção contínua

| Tarefa | Frequência |
|---|---|
| Backup completo do site | Mensal |
| Actualização de conteúdo (blog, portfólio) | Quinzenal |
| Verificação de links quebrados | Mensal |
| Revisão de performance (PageSpeed) | Trimestral |
| Renovação de domínio | Anual |
| Renovação de SSL (se manual) | Anual |
