# 2. Instalação e Configuração do Git

## 💾 Como instalar o Git

### 🪟 Windows

1. Abra o seu navegador e acesse: [https://git-scm.com](https://git-scm.com)  
2. Clique em **Download for Windows**  
3. O download será iniciado automaticamente. Após o término, abra o instalador  
4. Clique em **Next** nas etapas padrão  
5. Em "Select Components", clique em **Next**  
6. Na opção "Select Start Menu Folder", clique em **Next**  
   (ou marque **Don't create a Start Menu Folder** se preferir)  
7. Em "Choose the default editor used by Git", selecione seu editor favorito e clique em **Next**  
8. Continue clicando em **Next** até a opção **Install**  
9. Clique em **Install** e aguarde a instalação  
10. Após finalizar, clique em **Finish**  

> ✅ O Git está instalado no seu Windows!

---

### 🍎 macOS

A maneira mais simples de instalar o Git no macOS é utilizando o **Homebrew** (gerenciador de pacotes).

1. Abra o **Terminal**  
2. Digite o comando abaixo:
   ```bash
   brew install git
   ```
3. Aguarde a instalação  

> ✅ O Git está instalado no seu macOS!

---

### 🐧 Linux (Ubuntu/Debian)

1. Abra o **Terminal**  
2. Atualize os pacotes:
   ```bash
   sudo apt update
   ```
3. Instale o Git:
   ```bash
   sudo apt install git
   ```

> ✅ O Git está instalado no seu Linux!

---

## ⚙️ Como configurar o Git

Após instalar o Git, é importante configurar seu nome e e-mail, que serão usados nos commits.

1. Abra o **Terminal** ou **Git Bash** (no Windows)  
2. Digite os comandos abaixo, substituindo pelas suas informações:
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu@email.com"
   ```
3. Para verificar se foi salvo corretamente:
   ```bash
   git config --list
   ```

> ✅ Seu Git está configurado!

---

## ✅ Checando a Instalação

Para verificar se o Git está instalado corretamente:

1. No terminal, digite:
   ```bash
   git --version
   ```
2. Se aparecer algo como:
   ```
   git version 2.49.0
   ```
   Isso significa que a instalação foi concluída com sucesso!

---

## 📝 Dica

Caso queira alterar seu nome ou e-mail depois, basta repetir os comandos `git config --global` com os novos valores.
