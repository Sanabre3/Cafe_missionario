# ☕ Café Missionário — Igreja Missão Betesta Porto Novo

Landing page de evento para o **Café Missionário** da Igreja Missão Betesta Porto Novo.
Um site de página única (one-page) com tema de fé e missões, construído com HTML, CSS modular e Bootstrap 5.

> ⚠️ **Projeto de exercício.** Este é um trabalho de estudo/prática. Uma migração para **TypeScript** está planejada em breve.

---

## ✨ Funcionalidades

- **Layout responsivo** — adapta-se a desktop, tablet e celular
- **Navbar fixa** com efeito ao rolar a página e menu lateral (offcanvas) no mobile
- **Hero** em tela cheia com versículo e chamada de ação
- **Cardápio em abas** (Bebidas / Salgados / Doces) usando Bootstrap nav-pills
- **Seção Missão** com os passos *O Chamado · O Envio · O Impacto*
- **Animações de scroll reveal** via IntersectionObserver
- **Rolagem suave** entre as âncoras de navegação
- **Formulário de contato** estilizado

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|------------|-----|
| **HTML5** | Estrutura semântica |
| **CSS3** | Estilização (custom properties, grid, clamp, animações) |
| **Bootstrap 5.3.3** | Navbar, offcanvas, grid, cards, tabs, form, badges |
| **Bootstrap Icons 1.11.3** | Ícones |
| **Google Fonts** | Playfair Display · Lato · Dancing Script |
| **JavaScript (vanilla)** | Scroll reveal, navbar dinâmica, rolagem suave |

---

## 📁 Estrutura do Projeto

```
dev/
├── index.html              # Página principal (Bootstrap + classes semânticas)
├── main.css                # Ponto de entrada — apenas @imports
├── README.md               # Este arquivo
└── css/
    ├── variables.css       # CSS custom properties + overrides do Bootstrap
    ├── base.css            # Reset, utilitários, tipografia de seção, scroll reveal
    ├── navbar.css          # Navbar fixa + offcanvas mobile
    ├── hero.css            # Seção hero + animações (keyframes)
    ├── components.css      # Botões, cards do menu, tabs, form, social links
    ├── sections.css        # Sobre, destaques, missão, evento, footer
    └── responsive.css      # Media queries (992px · 768px · 576px)
```

### Por que CSS modular?

O `main.css` funciona apenas como ponto de entrada, importando cada arquivo por responsabilidade:

```css
@import url('css/variables.css');
@import url('css/base.css');
@import url('css/navbar.css');
@import url('css/hero.css');
@import url('css/components.css');
@import url('css/sections.css');
@import url('css/responsive.css');
```

Isso mantém cada arquivo curto, focado e fácil de manter.

---

## 🎨 Paleta de Cores

Tons quentes de café, definidos como CSS custom properties em `css/variables.css`:

| Variável | Cor | Uso |
|----------|-----|-----|
| `--espresso` | `#1C0E07` | Fundos escuros, texto |
| `--coffee` | `#6F3A1B` | Marrom de apoio |
| `--caramel` | `#C47D3A` | Destaques, hover |
| `--gold` | `#D4A847` | Acento principal |
| `--cream` | `#FDF6EC` | Fundo claro |
| `--beige` / `--sand` | `#F5E6D3` / `#E8D2B0` | Superfícies suaves |

---

## 🚀 Como Executar

Não há build step — é HTML/CSS estático.

1. Clone ou baixe o repositório
2. Abra o `index.html` no navegador

Ou, para servir localmente com live reload:

```bash
# Com a extensão Live Server do VS Code, ou:
npx serve .
```

---

## 🗺️ Roadmap

- [ ] **Migração para TypeScript** (em breve)
- [ ] Substituir mockups de imagem por fotos reais do evento
- [ ] Preencher dados reais (data, endereço, redes sociais)
- [ ] Integrar o formulário de contato a um backend

---

## 📄 Licença

Projeto de uso interno / educacional da Igreja Missão Betesta Porto Novo.
