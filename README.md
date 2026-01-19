# full-stack

<img src="https://coodesh.com/blog/wp-content/uploads/2022/07/como-dominar-o-git-scaled.jpg">

````markdown
# 📘 Tutorial de Comandos Git

Este tutorial apresenta os principais comandos do **Git** para versionamento de código, desde a configuração inicial até o trabalho com repositórios remotos.

O **Git** é um sistema de controle de versão distribuído que permite acompanhar mudanças no código, manter histórico e colaborar em equipe.

---

## 🔧 Instalação do Git

Para verificar se o Git já está instalado:
```bash
git --version
````

Instalação:

* Windows / macOS: [https://git-scm.com](https://git-scm.com)
* Linux (Debian/Ubuntu):

```bash
sudo apt install git
```

---

## ⚙️ Configuração Inicial

Configure seu nome e e-mail (obrigatório para commits):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@email.com"
```

Verificar configurações:

```bash
git config --list
```

---

## 📁 Criando um Repositório

Inicializar um repositório local:

```bash
git init
```

Clonar um repositório existente:

```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 📄 Status e Histórico

Verificar o estado dos arquivos:

```bash
git status
```

Visualizar histórico de commits:

```bash
git log
```

Histórico resumido:

```bash
git log --oneline
```

---

## ➕ Adicionando Arquivos (Stage)

Adicionar um arquivo específico:

```bash
git add arquivo.txt
```

Adicionar todos os arquivos:

```bash
git add .
```

---

## 💾 Criando Commits

Criar um commit:

```bash
git commit -m "Descrição da alteração"
```

---

## 🌿 Trabalhando com Branches

Criar uma branch:

```bash
git branch nome-da-branch
```

Trocar de branch:

```bash
git checkout nome-da-branch
```

Forma moderna:

```bash
git switch nome-da-branch
```

Criar e trocar de branch:

```bash
git checkout -b nova-branch
```

Listar branches:

```bash
git branch
```

---

## 🔀 Merge (Unir Branches)

Unir uma branch à atual:

```bash
git merge nome-da-branch
```

---

## ☁️ Repositório Remoto

Adicionar repositório remoto:

```bash
git remote add origin https://github.com/usuario/repositorio.git
```

Ver repositórios remotos:

```bash
git remote -v
```

---

## ⬆️ Enviando Alterações (Push)

Enviar commits:

```bash
git push origin main
```

Primeiro push:

```bash
git push -u origin main
```

---

## ⬇️ Atualizando Código (Pull)

Atualizar repositório local:

```bash
git pull origin main
```

---

## ♻️ Desfazendo Alterações

Descartar alterações locais:

```bash
git checkout -- arquivo.txt
```

Remover arquivo do stage:

```bash
git reset arquivo.txt
```

Desfazer último commit (mantendo arquivos):

```bash
git reset --soft HEAD~1
```

---

## 🧹 Arquivo `.gitignore`

Ignora arquivos no versionamento. Exemplo:

```txt
node_modules/
.env
dist/
*.log
```

---

## 🚀 Fluxo Básico de Trabalho

```text
1. git status
2. git add .
3. git commit -m "mensagem"
4. git pull
5. git push
```

---

## 📚 Comandos Úteis

```bash
git diff
git stash
git stash pop
git fetch
```

---

## ✅ Conclusão

Com estes comandos, você já consegue versionar projetos, trabalhar com branches e colaborar em equipe usando Git.

