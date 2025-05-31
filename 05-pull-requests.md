# 🌐 GitHub e Pull Requests

## 🧭 O que é o GitHub?

O GitHub é uma plataforma online que permite *armazenar repositórios Git na nuvem* e facilita a *colaboração entre desenvolvedores*. Ele oferece ferramentas visuais para acompanhar histórico de commits, branches, issues e pull requests.

---

## 🌱 Fluxo de trabalho com GitHub (Colaboração)

Quando trabalhamos em grupo usando GitHub, o processo mais comum é:

1. Um membro cria o *repositório principal* no GitHub.
2. Os outros membros *fazem um fork* (cópia) desse repositório para suas contas.
3. Cada um *clona* seu fork para trabalhar localmente.
4. Após concluir uma tarefa, o membro envia suas alterações para o *fork* com git push.
5. Em seguida, ele *abre um Pull Request* (PR) para solicitar a inclusão de suas mudanças no repositório principal.
6. Outro membro do grupo (ou o responsável) *revisa o PR* e faz o *merge* se estiver tudo certo.

---

## 🧪 Fork vs Clone

| Termo | Definição |
|------|-----------|
| Fork | Cópia do repositório na sua conta GitHub (online). Ideal para colaboração. |
| Clone | Cópia do repositório (ou do seu fork) no seu computador local. |

---

## 🔁 Criando um Pull Request (PR)

Depois de editar seu código em uma branch no seu fork:

1. Acesse seu fork no GitHub.
2. Vá até a aba *Pull Requests*.
3. Clique em *New Pull Request*.
4. Compare sua branch com a branch principal do repositório original.
5. Adicione um título e uma descrição explicando suas mudanças.
6. Clique em *Create Pull Request*.

Agora sua contribuição pode ser avaliada por outro membro!

---

## ✅ Revisando e Fazendo Merge de um PR

1. Vá até a aba *Pull Requests* no repositório principal.
2. Clique em um PR pendente.
3. Leia a descrição e revise os arquivos modificados.
4. Se tudo estiver certo:
   - Clique em *Merge pull request*.
   - Confirme clicando em *Confirm merge*.
5. Após o merge, é possível *deletar a branch* usada para o PR.

---

## 🧨 E se houver conflitos no PR?

Caso existam alterações incompatíveis entre o PR e a branch principal, o GitHub sinaliza um conflito.  
Quem criou o PR precisará:

- Fazer pull das alterações mais recentes do repositório principal.
- Resolver os conflitos localmente.
- Fazer um novo push para atualizar o PR.

---

## 📌 Dica de boas práticas

- Sempre use *branches* diferentes para cada nova funcionalidade.
- Escreva *mensagens claras* no título e descrição dos Pull Requests.
- Faça revisões com atenção antes de fazer o merge.