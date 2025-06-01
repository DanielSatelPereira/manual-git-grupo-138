# 3. Comandos Básicos do Git

Este módulo apresenta os comandos essenciais para começar a usar o Git em seus projetos locais. Todos os exemplos foram feitos em um repositório de teste.

---

## 🧱 `git init` – Inicializar um repositório

Cria um repositório Git dentro de uma pasta.

```bash
mkdir projeto
cd projeto
git init
```

Isso cria uma pasta oculta chamada `.git`, onde o Git armazena todo o histórico do projeto.

---

## 📄 `git status` – Verificar o status dos arquivos

Mostra o estado atual dos arquivos no repositório (se estão modificados, não rastreados, etc).

```bash
git status
```

Exemplo de saída:

```
On branch main

Untracked files:
  (use "git add <file>..." to include in what will be committed)
    index.html

nothing added to commit but untracked files present
```

---

## ➕ `git add` – Adicionar arquivos à área de preparação

Adiciona arquivos à *staging area* (área de preparação), deixando-os prontos para serem commitados.

```bash
git add nome-do-arquivo
```

Exemplo:

```bash
git add index.html
```

Adicionar todos os arquivos de uma vez:

```bash
git add .
```

---

## 📝 `git commit` – Salvar alterações no histórico

Registra as mudanças preparadas com uma mensagem descritiva.

```bash
git commit -m "mensagem explicando a mudança"
```

Exemplo:

```bash
git commit -m "feat: adiciona estrutura inicial do HTML"
```

---

## 📚 `git log` – Ver o histórico de commits

Exibe todos os commits realizados no repositório com detalhes.

```bash
git log
```

Exemplo de saída:

```
commit 9fceb02a...
Author: Ryan Alexandre <RyanF4k3@UmEmail.com>
Date:   Sat May 25 14:30:21 2025 -0300

    feat: adiciona estrutura inicial do HTML
```

---

## 🖼️ Simulação com Captura de Tela

> *[Inserir aqui uma imagem do terminal após rodar `git status`, mostrando arquivos modificados]*

---

## ✅ Resumo

| Comando       | Função                                     |
|---------------|---------------------------------------------|
| `git init`    | Inicia o repositório Git                   |
| `git status`  | Mostra arquivos modificados e rastreados   |
| `git add`     | Adiciona arquivos à área de preparação     |
| `git commit`  | Salva os arquivos com uma mensagem         |
| `git log`     | Mostra o histórico de commits              |
