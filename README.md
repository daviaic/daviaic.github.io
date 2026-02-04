# Site Acadêmico Pessoal

## 📁 Estrutura de Arquivos

```
seu-site/
│
├── index.html              # Página principal
├── publications.html       # Página de publicações
├── activities.html         # Página de atividades
├── contact.html           # Página de contato
├── style.css              # Estilos CSS
├── script.js              # JavaScript para interatividade
├── cv.pdf                 # Seu currículo (você precisa adicionar)
│
└── assets/
    └── img/
        └── photo.jpg      # Sua foto de perfil (você precisa adicionar)
```

## 🚀 Como Usar

### 1. Personalizar o Conteúdo

#### Informações Básicas (em todos os arquivos HTML):
- Substitua `"Seu Nome Completo"` pelo nome do seu amigo
- Substitua `"Pesquisador"` pelo título apropriado
- Atualize `"[Nome do Fotógrafo]"` pelo crédito da foto

#### Página Principal (index.html):
- Atualize a biografia com informações reais
- Adicione links para projetos, orientadores e instituições
- Personalize os parágrafos sobre pesquisa

#### Página de Publicações (publications.html):
- Adicione as publicações reais
- Inclua links para PDFs, DOIs, arXiv, código, etc.
- Organize por ordem cronológica (mais recente primeiro)

#### Página de Atividades (activities.html):
- Liste conferências, workshops revisados
- Adicione experiência de ensino
- Inclua palestras e participações em eventos

#### Página de Contato (contact.html):
- Atualize o email
- Adicione o endereço da universidade/instituição
- Inclua links para Google Scholar, ORCID, GitHub, LinkedIn

### 2. Adicionar Foto de Perfil

Crie a pasta `assets/img/` e adicione a foto:
```
mkdir -p assets/img
```
Depois coloque a foto de perfil como `assets/img/photo.jpg`

**Dica:** Use uma foto quadrada ou em formato retrato para melhor resultado.

### 3. Adicionar CV

Adicione o arquivo PDF do currículo na raiz do projeto com o nome `cv.pdf`.

### 4. Personalizar Cores (Opcional)

Edite o arquivo `style.css` na seção de variáveis CSS (início do arquivo):

```css
:root {
    --color-primary: #2c3e50;      /* Cor principal dos títulos */
    --color-accent: #3498db;        /* Cor dos links e destaques */
    --color-text: #333333;          /* Cor do texto principal */
    /* ... outras variáveis ... */
}
```

### 5. Publicar no GitHub Pages

#### Opção A: Via Interface Web do GitHub

1. Vá até o repositório no GitHub
2. Clique em "Add file" > "Upload files"
3. Arraste todos os arquivos (HTML, CSS, JS)
4. Crie a pasta `assets/img` e faça upload da foto
5. Faça upload do CV (cv.pdf)
6. Commit das mudanças
7. Vá em Settings > Pages
8. Em "Source", selecione "main" branch e pasta "/ (root)"
9. Clique em "Save"
10. O site estará disponível em: `https://[usuario].github.io/[nome-do-repo]/`

#### Opção B: Via Git (Linha de Comando)

```bash
# Clone o repositório (se ainda não fez)
git clone https://github.com/[usuario]/[nome-do-repo].git
cd [nome-do-repo]

# Copie todos os arquivos do site para o repositório
# (copie: index.html, publications.html, activities.html, contact.html, style.css, script.js, cv.pdf)
# (copie a pasta: assets/)

# Adicione os arquivos
git add .

# Commit
git commit -m "Adiciona site pessoal"

# Push para o GitHub
git push origin main

# Ative o GitHub Pages nas configurações do repositório
```

## 🎨 Características do Design

- **Responsivo:** Funciona perfeitamente em desktop, tablet e celular
- **Minimalista:** Design clean e profissional
- **Animações Sutis:** Transições suaves e efeitos ao scroll
- **Tipografia Elegante:** Fontes Google Fonts (Crimson Pro + Work Sans)
- **Navegação Mobile:** Menu hambúrguer para dispositivos móveis
- **Performance:** Otimizado e leve

## 🔧 Customizações Avançadas

### Adicionar Google Analytics (Opcional)

Adicione antes do `</head>` em cada HTML:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=SEU-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'SEU-ID');
</script>
```

### Adicionar Mais Páginas

Duplique qualquer arquivo HTML existente e personalize o conteúdo. Não esqueça de:
1. Atualizar o `<title>`
2. Adicionar o link no menu de navegação
3. Manter a mesma estrutura de header e footer

## 📱 Testando Localmente

Para testar o site localmente antes de publicar:

1. Abra qualquer arquivo HTML diretamente no navegador, OU
2. Use um servidor local simples:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Depois acesse: `http://localhost:8000`

## ⚡ Dicas Importantes

1. **Otimize as imagens:** Comprima a foto de perfil antes do upload (recomendado: max 500KB)
2. **Links válidos:** Verifique que todos os links para publicações estão funcionando
3. **Atualize regularmente:** Mantenha publicações e atividades sempre atualizadas
4. **SEO:** Adicione meta tags descritivas em cada página
5. **Acessibilidade:** O site já está otimizado, mas sempre teste a navegação por teclado

## 🆘 Problemas Comuns

**A foto não aparece:**
- Verifique se o caminho está correto: `assets/img/photo.jpg`
- Confirme que a pasta foi criada corretamente

**Página não está estilizada:**
- Verifique se o arquivo `style.css` está na mesma pasta que os HTML
- Confirme que o link no `<head>` está correto

**Menu mobile não funciona:**
- Verifique se o arquivo `script.js` está carregando corretamente
- Abra o console do navegador (F12) para ver erros

## 📝 Licença

Use livremente para criar seu site acadêmico!

---

**Desenvolvido com ❤️ para pesquisadores acadêmicos**
