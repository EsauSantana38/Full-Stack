# Full-Stack

# 📘 Tutorial de Comandos Git para Versionamento de Código com GitHub

Este tutorial apresenta os **principais comandos do Git**, explicados passo a passo, para você versionar seus projetos e publicá-los no **GitHub**. Ideal para iniciantes.

---

## 📌 O que é Git?

O **Git** é um sistema de controle de versão distribuído que permite:

* Controlar alterações no código
* Trabalhar em equipe
* Voltar versões antigas do projeto

## 🌐 O que é GitHub?

O **GitHub** é uma plataforma online que armazena repositórios Git, permitindo colaboração, backup e compartilhamento de código.

---

## 🔧 Instalação do Git

### 🔹 Windows

Baixe em: [https://git-scm.com](https://git-scm.com)

### 🔹 Verificar instalação

```bash
git --version
```

---

## 👤 Configuração Inicial do Git

Configure seu nome e e-mail (use o mesmo do GitHub):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@email.com"
```

Verificar configurações:

```bash
git config --list
```

---

## 📁 Criando um Repositório Local

Entre na pasta do projeto:

```bash
cd caminho/do/projeto
```

Inicialize o Git:

```bash
git init
```

📌 Isso cria a pasta oculta `.git`

---

## 📄 Verificando Status dos Arquivos

```bash
git status
```

Mostra:

* Arquivos modificados
* Arquivos não rastreados
* Arquivos prontos para commit

---

## ➕ Adicionando Arquivos ao Versionamento

Adicionar um arquivo específico:

```bash
git add arquivo.txt
```

Adicionar todos os arquivos:

```bash
git add .
```

---

## 💾 Salvando Alterações (Commit)

```bash
git commit -m "Mensagem descrevendo a alteração"
```

📌 O commit cria um **ponto de salvamento** no histórico.

---

## 🕘 Histórico de Commits

```bash
git log
```

Versão resumida:

```bash
git log --oneline
```

---

## 🌿 Trabalhando com Branches

### Criar uma branch

```bash
git branch nome-da-branch
```

### Trocar de branch

```bash
git checkout nome-da-branch
```

### Criar e trocar ao mesmo tempo

```bash
git checkout -b nova-branch
```

### Listar branches

```bash
git branch
```

---

## 🔀 Unindo Branches (Merge)

```bash
git merge nome-da-branch
```

📌 Executar na branch que **receberá** as alterações.

---

## 🌍 Conectando ao GitHub

### Criar repositório no GitHub

* Não marque README (se já existir local)

### Conectar repositório local ao remoto

```bash
git remote add origin https://github.com/usuario/repositorio.git
```

Verificar conexão:

```bash
git remote -v
```

---

## 🚀 Enviando Código para o GitHub (Push)

```bash
git push -u origin main
```

📌 `-u` define a branch padrão

---

## ⬇️ Baixando Código do GitHub

### Clonar repositório

```bash
git clone https://github.com/usuario/repositorio.git
```

### Atualizar repositório local

```bash
git pull
```

---

## ❌ Desfazendo Alterações

### Desfazer alterações não adicionadas

```bash
git checkout -- arquivo.txt
```

### Remover arquivo do stage

```bash
git reset arquivo.txt
```

### Voltar para commit anterior

```bash
git reset --hard codigo_do_commit
```

⚠️ Atenção: esse comando apaga alterações!

---

## 📄 Arquivo .gitignore

Usado para ignorar arquivos no versionamento.

Exemplo:

```text
/node_modules
.env
*.log
```

---

## 📌 Fluxo Básico de Trabalho com Git

1. Modificar arquivos
2. `git status`
3. `git add .`
4. `git commit -m "mensagem"`
5. `git push`

---

## ✅ Boas Práticas

* Commits pequenos e frequentes
* Mensagens claras
* Usar branches para novas funcionalidades
* Nunca subir senhas ou dados sensíveis

---

## 📚 Comandos Mais Usados (Resumo)

| Comando    | Função             |
| ---------- | ------------------ |
| git init   | Inicia repositório |
| git status | Ver status         |
| git add .  | Adiciona arquivos  |
| git commit | Salva versão       |
| git log    | Histórico          |
| git branch | Gerenciar branches |
| git merge  | Unir branches      |
| git push   | Enviar para GitHub |
| git pull   | Atualizar código   |

---

## 🎯 Conclusão

Com esses comandos você já consegue versionar seus projetos, trabalhar em equipe e usar o GitHub com segurança.

