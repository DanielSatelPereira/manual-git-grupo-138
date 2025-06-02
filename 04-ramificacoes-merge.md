# 🌿 Branches e Merge
<p align="center">
  <img src="/imagens/imagem-exemplo-branchs.png" alt="Exemplo de Branches" />
</p>



## 📌 4.1 - O que são branches

Branches (ramificações) permitem que você desenvolva funcionalidades isoladas sem afetar a linha principal do código (geralmente a `main` ou `master`).  
Ao criar um branch, você está copiando o estado atual do projeto para trabalhar em paralelo, podendo depois juntar as alterações com o `merge`.

Essa abordagem evita conflitos frequentes e melhora o fluxo de colaboração em equipe.

---

## ✨ 4.2 - Criar, mudar e deletar branches

### ✅ Criar um branch

- **Via GitHub (interface web):**
  - Vá até a página do repositório.
  - No menu de branches, clique em **Exibir todos os branches**.
  - Clique em **Criar nova branch**.

- **Via terminal (linha de comando):**
  ```bash
  git branch nome-da-branch
  git checkout nome-da-branch
  ```
  Ou diretamente:
  ```bash
  git checkout -b nome-da-branch
  ```

---

### 🔁 Alternar entre branches

- **Via GitHub:**
  - Clique no menu suspenso de branch e selecione a branch desejada.

- **Via terminal:**
  ```bash
  git checkout nome-da-branch
  ```

---

### 🗑️ Deletar uma branch

- **Via GitHub:**
  - Vá em **Exibir todos os branches**.
  - Clique na lixeira ao lado do branch desejado (só se não tiver pull request aberto).

- **Via terminal:**
  ```bash
  git branch -d nome-da-branch
  ```

---

## 🔀 4.3 - `git merge` e como lidar com conflitos

### O que é `git merge`?

O comando `git merge` une as alterações de um branch (geralmente de uma funcionalidade) ao branch atual.  
Exemplo:
```bash
git merge nome-da-branch
```

### 🧨 Por que ocorrem conflitos?

Conflitos acontecem quando:
- Duas pessoas alteram a **mesma linha** de um arquivo.
- Uma altera e a outra **deleta** o mesmo arquivo.

O Git não consegue decidir automaticamente qual versão manter.

---

### ✅ Como resolver conflitos

**Passo a passo:**
1. Abra o terminal (Git Bash).
2. Navegue até o repositório.
3. Liste os arquivos em conflito:
   ```bash
   git status
   ```
4. Abra os arquivos conflitantes em seu editor de texto (ex: VS Code).
5. Procure os marcadores:
   ```
   <<<<<<< HEAD
   [Seu código]
   =======
   [Código do outro branch]
   >>>>>>> nome-da-branch
   ```
6. Escolha **qual versão manter** ou combine as duas.
7. Remova os marcadores `<<<<<<<`, `=======`, `>>>>>>>`.
8. Adicione as alterações:
   ```bash
   git add nome-do-arquivo
   ```
9. Faça o commit:
   ```bash
   git commit -m "fix: resolve conflitos de merge entre main e nome-da-branch"
   ```

---

## ✅ Resumo

| Comando                          | Função                                             |
|----------------------------------|----------------------------------------------------|
| `git branch nome`                | Cria uma nova branch                               |
| `git checkout nome`              | Troca para a branch desejada                       |
| `git branch -d nome`             | Deleta a branch                                    |
| `git merge nome`                 | Junta a branch atual com a especificada            |
| (resolução de conflito manual)   | Escolhe entre as versões de código em conflito     |
