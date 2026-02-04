# 🚀 GUIA RÁPIDO: Como Fazer Upload para o GitHub

## Passo a Passo Visual (Interface Web)

### 1. Prepare os Arquivos Localmente

Organize todos os arquivos nesta estrutura:
```
📁 Pasta do Site/
├── 📄 index.html
├── 📄 publications.html
├── 📄 activities.html
├── 📄 contact.html
├── 📄 style.css
├── 📄 script.js
├── 📄 cv.pdf (adicione seu CV aqui!)
└── 📁 assets/
    └── 📁 img/
        └── 🖼️ photo.jpg (adicione sua foto aqui!)
```

### 2. Acesse o Repositório no GitHub

1. Vá para: `https://github.com/[usuario]/[nome-do-repositorio]`
2. Você deve estar como colaboradora

### 3. Faça Upload dos Arquivos

**Opção A - Upload direto (Recomendado para iniciantes):**

1. Clique no botão **"Add file"** (canto superior direito)
2. Selecione **"Upload files"**
3. Arraste TODOS os arquivos da pasta ou clique em "choose your files"
4. ⚠️ **IMPORTANTE:** Para manter a estrutura de pastas:
   - Primeiro faça upload dos arquivos da raiz (HTML, CSS, JS, PDF)
   - Depois, vá para "Add file" > "Create new file"
   - Digite: `assets/img/.gitkeep` (isso cria a pasta)
   - Commit
   - Entre na pasta `assets/img` e faça upload da foto

5. Na caixa "Commit changes" no final da página:
   - Adicione uma mensagem como: "Adiciona site pessoal inicial"
6. Clique em **"Commit changes"**

**Opção B - Upload através de commits individuais:**

Para cada arquivo:
1. "Add file" > "Create new file"
2. No campo de nome, digite o caminho completo (ex: `style.css`)
3. Cole o conteúdo do arquivo
4. Commit

### 4. Ativar GitHub Pages

1. No repositório, clique em **"Settings"** (última aba)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em **"Source"**:
   - Branch: selecione `main` (ou `master`)
   - Folder: selecione `/ (root)`
4. Clique em **"Save"**
5. Aguarde 1-2 minutos ⏱️

### 5. Acessar seu Site

Após alguns minutos, seu site estará disponível em:
```
https://[usuario].github.io/[nome-do-repositorio]/
```

Exemplo: `https://joaosilva.github.io/meu-site-academico/`

---

## ✅ Checklist Antes de Publicar

- [ ] Atualizei o nome em todos os arquivos HTML
- [ ] Adicionei minha biografia na página inicial
- [ ] Coloquei minhas publicações reais
- [ ] Atualizei informações de contato
- [ ] Adicionei minha foto de perfil (photo.jpg)
- [ ] Incluí meu CV (cv.pdf)
- [ ] Testei os links de navegação
- [ ] Revisei todo o conteúdo

---

## 🔄 Como Atualizar o Site Depois

Para fazer mudanças:

1. Acesse o arquivo no GitHub
2. Clique no ícone do lápis ✏️ (Edit)
3. Faça as alterações
4. Scroll até o final
5. Adicione uma mensagem de commit (ex: "Atualiza publicações")
6. Clique em "Commit changes"

As mudanças aparecerão no site em 1-2 minutos!

---

## 🆘 Problemas Comuns

### Site não aparece após ativar GitHub Pages
- Aguarde 5 minutos
- Verifique se o branch correto está selecionado
- Force refresh: Ctrl + Shift + R (ou Cmd + Shift + R no Mac)

### Imagens não aparecem
- Verifique se os nomes dos arquivos estão corretos
- Confirme que a estrutura de pastas está correta: `assets/img/photo.jpg`
- Nomes de arquivo são case-sensitive no GitHub Pages!

### CSS não está funcionando
- Verifique se o arquivo `style.css` foi carregado
- Confirme que está na mesma pasta que os HTMLs
- Limpe o cache do navegador

---

## 💡 Dicas Extras

1. **Domínio Personalizado** (opcional):
   - Em Settings > Pages, você pode adicionar um domínio próprio
   - Ex: `www.seu-nome.com`

2. **Proteja a branch main**:
   - Settings > Branches > Add rule
   - Isso evita exclusões acidentais

3. **Issues do GitHub**:
   - Use para fazer lista de tarefas (To-Do)
   - Ex: "Adicionar nova publicação"

---

**Boa sorte! 🎓✨**
