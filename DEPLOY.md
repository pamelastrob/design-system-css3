# Guia de Deploy - GitHub

**Desenvolvido por: Pamela Strob Mancegozo Lima**

## Como Publicar o Projeto no GitHub

### 1. Inicializar o Repositório Git

```bash
# Navegar até a pasta do projeto
cd "Adejo Desenvolvimento/Adejo Desenvovimento IA/Trabalhos Faculdade/Trabalho2"

# Inicializar repositório Git
git init

# Adicionar todos os arquivos
git add .

# Criar commit inicial
git commit -m "feat: Sistema de Design CSS3 - Entrega II"
```

### 2. Criar Repositório no GitHub

1. Acesse [GitHub](https://github.com)
2. Clique em "New repository"
3. Nome do repositório: `design-system-css3`
4. **IMPORTANTE**: Marque como **PÚBLICO**
5. NÃO inicialize com README, .gitignore ou license
6. Clique em "Create repository"

### 3. Conectar e Fazer Push

```bash
# Adicionar remote
git remote add origin https://github.com/SEU-USUARIO/design-system-css3.git

# Verificar branch
git branch -M main

# Fazer push
git push -u origin main
```

### 4. Configurar GitHub Pages (Opcional)

1. No repositório, vá em **Settings**
2. Role até **Pages**
3. Em "Source", selecione **main branch**
4. Salve

Seu site estará em: `https://SEU-USUARIO.github.io/design-system-css3/`

### 5. Verificar se o Link Está Público

⚠️ **CRÍTICO**: O repositório DEVE estar público para a correção!

- Vá em Settings → Repositório público
- Ou acesse: `https://github.com/SEU-USUARIO/design-system-css3`
- Qualquer pessoa deve conseguir acessar sem login

## Checklist de Entrega

Antes de entregar, verifique:

- [ ] Repositório está público no GitHub
- [ ] Link GitHub foi fornecido ao professor
- [ ] Todos os arquivos CSS estão na pasta `css/`
- [ ] Pasta `imagens/` existe (mesmo que vazia)
- [ ] `index.html` está na raiz
- [ ] `README.md` está na raiz
- [ ] CSS é modular e organizado
- [ ] Menu hambúrguer funciona em mobile
- [ ] Grid responsivo funciona
- [ ] Todos os componentes estão estilizados
- [ ] 5+ breakpoints estão implementados

## Estrutura Esperada no GitHub

```
design-system-css3/
├── css/
│   ├── base/
│   │   ├── _variables.css
│   │   └── _reset.css
│   ├── components/
│   │   ├── _alerts.css
│   │   ├── _badges.css
│   │   ├── _buttons.css
│   │   ├── _cards.css
│   │   ├── _forms.css
│   │   └── _modals.css
│   ├── layout/
│   │   ├── _footer.css
│   │   ├── _grid.css
│   │   ├── _header.css
│   │   └── _hero.css
│   ├── utils/
│   │   └── _utilities.css
│   └── style.css
├── imagens/
├── index.html
├── README.md
├── .gitignore
└── .gitattributes
```

## Link para Incluir na Entrega

```
https://github.com/SEU-USUARIO/design-system-css3
```

Substitua `SEU-USUARIO` pelo seu username do GitHub.

## Avisos Importantes

1. **Repositório DEVE estar PÚBLICO** - Professor precisa acessar
2. **Não incluir** repositórios de outras atividades
3. **Link direto** ao repositório específico desta entrega
4. **Todas as pastas** devem existir, mesmo que vazias
5. **HTML deve apontar** para `css/style.css`

## Dicas

- Comit frequente: `git add . && git commit -m "mensagem"`
- Histórico limpo facilita correção
- Use `git status` para verificar mudanças
- Use `git log` para ver histórico

## Comandos Úteis

```bash
# Ver status
git status

# Adicionar arquivos
git add .

# Fazer commit
git commit -m "descrição da mudança"

# Ver histórico
git log --oneline

# Push para GitHub
git push origin main

# Ver remotes
git remote -v
```

## Boa Sorte!

Seu projeto está completo e pronto para entrega!

