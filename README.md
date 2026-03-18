# ✦ portfolio-ui-kit

> A clean, minimal UI design system with dark & light mode — built with pure HTML, CSS and vanilla JS.

![Preview](https://img.shields.io/badge/version-1.0.0-brightgreen?style=flat-square&labelColor=0d0d0f&color=c8f07a)
![HTML](https://img.shields.io/badge/HTML-pure-orange?style=flat-square&labelColor=0d0d0f&color=f87171)
![CSS](https://img.shields.io/badge/CSS-variables-blue?style=flat-square&labelColor=0d0d0f&color=7eb8f7)
![License](https://img.shields.io/badge/license-MIT-purple?style=flat-square&labelColor=0d0d0f&color=5ee8d0)

---

## ✦ Preview

| Dark Mode | Light Mode |
|-----------|------------|
| ![dark](.github/preview-dark.png) | ![light](.github/preview-light.png) |

> **Live demo:** [herbertis.github.io/portfolio-ui-kit](https://herbertis.github.io/portfolio-ui-kit/)

---

## ✦ O que é

**portfolio-ui-kit** é um design system single-file — sem frameworks, sem dependências, sem build step. Um arquivo HTML com todos os tokens, componentes e interações prontos para usar como referência visual ou como base de projetos.

Pensado para portfolios e projetos pessoais que precisam de uma UI consistente, clean e com personalidade.

---

## ✦ Features

- **Dark / Light mode** — toggle suave com transição em todos os tokens simultaneamente
- **Scroll reveal** — cada seção aparece com animação ao entrar na viewport via `IntersectionObserver`
- **Scroll progress bar** — barra de progresso no topo da página
- **Zero dependências** — HTML + CSS Variables + Vanilla JS puro
- **Single file** — tudo em um único `index.html`
- **Totalmente responsivo** — funciona em mobile, tablet e desktop

---

## ✦ Componentes incluídos

| Categoria | Componentes |
|-----------|-------------|
| **Tokens** | Colors, Typography, Spacing, Radius, Shadows |
| **Buttons** | Primary, Teal, Soft, Outline, Ghost, Surface, Danger, Danger Solid |
| **Button States** | Sizes (XS→XL), Pill, Icon, Loading, Disabled |
| **Inputs** | Text, Email, Password, Search, Textarea, Select |
| **Input States** | Default, Focus, Error, Success, Disabled |
| **Input Addons** | Icon left/right, Prefix text, Action button |
| **Controls** | Checkbox, Radio, Toggle/Switch, Range slider |
| **Badges** | Green, Teal, Rose, Amber, Blue, Muted — rounded & square |
| **Cards** | Default, Accent hover, Teal hover |
| **Alerts** | Success, Info, Warning, Error |
| **Progress** | Thin (2px), Default (4px), Medium (6px), Thick (8px) + shimmer |
| **Avatars** | XS → LG, colored variants, avatar stack |

---

## ✦ Tipografia

| Font | Uso | Peso |
|------|-----|------|
| **Fraunces** | Display, headings | 300, 400 (serif elegante) |
| **Geist** | Body, labels, buttons | 300, 400, 500, 600 |
| **Geist Mono** | Code, mono, labels | 300, 400, 500 |

---

## ✦ Paleta de cores

```css
/* Dark mode */
--accent:  #c8f07a   /* Lime green — primary */
--teal:    #5ee8d0   /* Teal — secondary */
--rose:    #f87171   /* Rose — danger */
--amber:   #f5b94e   /* Amber — warning */
--blue:    #7eb8f7   /* Blue — info */

/* Light mode (adapta automaticamente) */
--accent:  #4a8c1c
--teal:    #0f7c68
--rose:    #c53030
--amber:   #b45309
--blue:    #2563b0
```

---

## ✦ Como usar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/portfolio-ui-kit.git
cd portfolio-ui-kit
```

### 2. Abra direto no browser

```bash
open index.html
# ou simplesmente arraste o arquivo para o browser
```

### 3. Copie os tokens CSS

Todos os tokens ficam no bloco `:root` e `[data-theme]` no topo do arquivo. Copie para o seu projeto:

```css
[data-theme="dark"] {
  --bg:      #0d0d0f;
  --accent:  #c8f07a;
  --teal:    #5ee8d0;
  /* ... */
}

[data-theme="light"] {
  --bg:      #f8f7f4;
  --accent:  #4a8c1c;
  /* ... */
}
```

### 4. Copie os componentes

Cada componente é HTML + classe CSS pura. Exemplo de botão:

```html
<!-- Primary button -->
<button class="btn btn-primary btn-md">Click me</button>

<!-- Outline pill -->
<button class="btn btn-outline btn-lg btn-pill">Learn more</button>

<!-- Icon button -->
<button class="btn btn-icon btn-surface btn-md">...</button>
```

---

## ✦ Estrutura do projeto

```
portfolio-ui-kit/
├── index.html          ← tudo aqui (tokens + componentes + JS)
├── README.md
└── .github/
    ├── preview-dark.png
    └── preview-light.png
```

---

## ✦ Deploy no GitHub Pages

1. Vá em **Settings → Pages**
2. Source: `Deploy from a branch`
3. Branch: `main` / `root`
4. Salve — em ~1 minuto estará live em:

```
https://seu-usuario.github.io/portfolio-ui-kit
```

---

## ✦ Customização rápida

Para mudar o accent color do sistema inteiro, basta alterar duas variáveis:

```css
[data-theme="dark"]  { --accent: #sua-cor; --accent-soft: rgba(sua-cor, 0.10); }
[data-theme="light"] { --accent: #sua-cor-light; }
```

Todos os botões, inputs focus, badges, progress bars e toggles atualizam automaticamente.

---

## ✦ Roadmap

- [ ] Versão React com componentes isolados
- [ ] Figma file com todos os tokens e componentes
- [ ] Modo high contrast
- [ ] Animações de entrada configuráveis via CSS custom property
- [ ] Pacote npm

---

## ✦ Licença

MIT — use à vontade, créditos são bem-vindos mas não obrigatórios.

---

<div align="center">

Feito com cuidado por [você](https://github.com/seu-usuario) · **portfolio-ui-kit** v1.0.0

</div>
