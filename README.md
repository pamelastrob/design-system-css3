# Design System CSS3 - Interface Moderna

Desenvolvido por: Pamela Strob Mancegozo Lima

## Descricao do Projeto

Sistema de design responsivo desenvolvido com CSS3, incluindo:
- Variaveis CSS
- Layouts responsivos com Flexbox e Grid
- Componentes interativos
- Breakpoints para dispositivos
- Grid de 12 colunas
- Menu para mobile
- Componentes: Cards, Botoes, Formularios, Alerts

## Objetivos da Entrega

Entrega II do projeto, focada em:
1. Sistema de Design com variaveis CSS, cores, tipografia e espacamento
2. Layouts Responsivos com Flexbox e CSS Grid
3. Navegacao com menu e submenu
4. Componentes de Interface com estados visuais

## Estrutura de Pastas

```
/
├── css/
│   ├── base/
│   │   ├── _variables.css    # Variaveis CSS
│   │   └── _reset.css         # Reset basico
│   ├── layout/
│   │   ├── _grid.css          # Sistema de grid
│   │   ├── _header.css        # Header
│   │   ├── _hero.css          # Secao hero
│   │   └── _footer.css        # Footer
│   ├── components/
│   │   ├── _buttons.css       # Botoes
│   │   ├── _cards.css         # Cards
│   │   ├── _forms.css         # Formularios
│   │   ├── _badges.css        # Badges
│   │   ├── _alerts.css        # Alerts
│   │   └── _modals.css        # Modals
│   ├── utils/
│   │   └── _utilities.css     # Classes utilitarias
│   └── style.css              # Arquivo principal
├── imagens/                   # Pasta para imagens
├── index.html                 # Pagina HTML principal
└── README.md                  # Documentacao
```

## Sistema de Design

### Paleta de Cores

O sistema inclui 8 cores organizadas em categorias:

- Primarias: primary, primary-light, primary-dark
- Secundarias: secondary, secondary-light, secondary-dark  
- Neutras: neutral-50 a neutral-900
- Status: Success, Error, Warning, Info

### Tipografia

5 tamanhos de fonte:
- xs: 12px
- sm: 14px
- base: 16px
- lg: 18px
- xl: 20px
- 2xl: 24px
- 3xl: 30px
- 4xl: 36px
- 5xl: 48px
- 6xl: 60px

### Espacamento

Sistema baseado em 8px:
- xs: 8px
- sm: 16px
- md: 24px
- lg: 32px
- xl: 48px
- 2xl: 64px

## Breakpoints

O sistema define 5 breakpoints:

- xs: 320px (Mobile Pequeno)
- sm: 640px (Mobile)
- md: 768px (Tablet)
- lg: 1024px (Desktop)
- xl: 1280px (Desktop Grande)
- 2xl: 1536px (Desktop Muito Grande)

## Grid System

Sistema de grid de 12 colunas com classes responsivas:

```html
<div class="grid">
  <div class="grid-12 md-grid-6 lg-grid-4">Coluna 1</div>
  <div class="grid-12 md-grid-6 lg-grid-4">Coluna 2</div>
  <div class="grid-12 md-grid-6 lg-grid-4">Coluna 3</div>
</div>
```

Classes disponiveis:
- grid-1 a grid-12
- Variantes: sm-grid, md-grid, lg-grid, xl-grid

## Componentes

### Botoes

Botoes com 4 estados visuais:
- hover
- focus
- active
- disabled

Variantes: Primary, Secondary, Outline, Ghost, Success, Error, Warning, Info
Tamanhos: xs, sm, lg, xl

```html
<button class="btn btn--primary btn--lg">Clique Aqui</button>
```

### Cards

Cards responsivos para projetos:

```html
<div class="card">
  <div class="card__image-wrapper">
    <img src="..." class="card__image">
  </div>
  <div class="card__content">
    <h3 class="card__title">Título</h3>
    <p class="card__description">Descrição...</p>
  </div>
</div>
```

### Formularios

Formularios estilizados com validacao visual:

```html
<div class="form-group">
  <label class="form-label">Email</label>
  <input type="email" class="form-input">
</div>
```

### Alerts

Componentes de feedback:

```html
<div class="alert alert--success">
  <div class="alert__content">
    <p class="alert__title">Sucesso!</p>
    <p class="alert__message">Operacao realizada.</p>
  </div>
</div>
```

Variantes: success, error, warning, info

### Badges

Sistema de tags:

```html
<span class="badge badge--primary">Nova</span>
```

## Navegacao

### Menu Mobile

Menu responsivo com botao hamburguer para dispositivos moveis.

### Submenu

Navegacao com submenu que funciona em desktop e mobile.

## Funcionalidades Interativas (JavaScript)

O projeto inclui JavaScript para funcionalidades dinamicas:
- Menu mobile com toggle
- Efeito de scroll no header
- Interacoes com componentes (modals, alerts)
- Navegacao suave entre secoes
- Validacao de formularios em tempo real

## Caracteristicas

Sistema de Design com variaveis CSS
Paleta de Cores com tons rosa
Tipografia com varios tamanhos de fonte
Espacamento baseado em 8px
CSS Grid de 12 colunas
Flexbox para componentes
Breakpoints para responsividade
Menu mobile interativo
Submenu dinamico
Cards responsivos
Botoes com estados
Formularios estilizados com validacao
Alerts para feedback
Badges para tags
Modals interativos
Foco visivel para acessibilidade
CSS modular
JavaScript para interatividade  

## Como Usar

1. Clone o repositório
2. Abra `index.html` no navegador
3. Explore os componentes e layouts

### Importar CSS

```html
<link rel="stylesheet" href="css/style.css">
```

### Estrutura Modular

O arquivo style.css importa todos os modulos:

```css
@import url('./base/_variables.css');
@import url('./base/_reset.css');
@import url('./layout/_grid.css');
```

## Estrutura CSS

- base: Reset, variaveis, estilos base
- layout: Header, footer, grid, hero
- components: Botoes, cards, formularios
- utils: Classes utilitarias
- style.css: Arquivo principal

## Especificacoes Tecnicas Obrigatorias - Atendidas

### Sistema de Design
- Design system consistente com variaveis CSS customizadas
- Paleta de cores com 8 cores (primarias, secundarias, neutras, status)
- Tipografia hierarquica com 5+ tamanhos de fonte
- Sistema de espacamento modular (8px, 16px, 24px, 32px, 48px, 64px)

### Leiautes Responsivos com Flexbox e Grid
- Leiaute principal usando CSS Grid para estrutura geral
- Flexbox para componentes internos e alinhamentos
- 5 breakpoints bem definidos (640px, 768px, 1024px, 1280px, 1536px)
- Sistema de grid customizado (12 colunas)
- Leiautes especificos para diferentes tipos de conteudo

### Navegacao Sofisticada e Interativa
- Menu principal responsivo com submenu dropdown
- Navegacao mobile com menu hamburguer

### Componentes de Interface
- Sistema de cards responsivos para projetos
- Botoes com estados visuais (hover, focus, active, disabled)
- Formularios estilizados com validacao visual
- Componentes de feedback (alerts, toasts, modals)
- Sistema de badges e tags para categorizacao

## Estrutura de Entrega

### CSS Organizados
- Estrutura de pastas organizada (pastas, HTML, imagens e CSS)
- Estrutura modular de CSS

### Forma de Entrega
- Link PUBLICO do projeto no GitHub: https://github.com/pamelastrob/design-system-css3
- Codigo fonte e arquivos HTML e imagens organizados em pastas
- Pasta css/ com todos os arquivos CSS modulares  

## Deploy

Este projeto pode ser hospedado em:
- GitHub Pages
- Netlify
- Vercel

## Licenca

Este projeto foi desenvolvido para fins educacionais.

## Desenvolvedor

Pamela Strob Mancegozo Lima

Desenvolvido como parte da atividade Experiencias Praticas - Linguagem de Estilo: Construindo Interfaces Web Modernas com CSS3 (Entrega II).

---

Este projeto demonstra conhecimento de CSS3 moderno, incluindo:
- Variaveis CSS
- Flexbox e Grid
- Animacoes
- Responsividade
- Componentes reutilizaveis
- Acessibilidade basica
- Design com paleta de cores rosa

