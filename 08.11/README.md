### 1. Branches (ou Ramificações)

No Git, uma **branch** é uma ramificação que permite criar uma "cópia paralela" do seu código. Isso facilita testar novos recursos ou resolver problemas sem interferir no código principal (geralmente na `main` ou `master`). Dessa forma, qualquer pessoa pode trabalhar sem afetar o trabalho dos outros.

### Comandos para Trabalhar com Branches

1. **Criar uma nova branch**: Use o comando `git checkout -b <nome-da-branch>`. Esse comando cria uma nova branch e já te move para ela. Substitua `<nome-da-branch>` por um nome que descreva o que você está desenvolvendo, como `nova-funcionalidade` ou `correcao-bug`.

   ```bash
   git checkout -b minha-nova-branch
   ```

2. **Verificar em qual branch você está**: Para ver a branch em que está, use o comando:

   ```bash
   git branch
   ```

   A branch ativa será destacada com um asterisco (`*`).

3. **Enviar a branch para o repositório remoto**: Quando estiver pronto para compartilhar suas mudanças, faça o push da sua branch para o repositório remoto:

   ```bash
   git push origin minha-nova-branch
   ```

---

### 2. Pull Request (PR)

O **Pull Request** é uma forma de avisar a equipe que uma funcionalidade está pronta para ser revisada e, possivelmente, integrada ao código principal. Outros membros da equipe podem revisar as alterações antes que elas sejam mescladas com a branch principal, garantindo que o código está correto e consistente.

### Passo a Passo para Criar um Pull Request

1. **Fazer o Push da Branch**: Primeiro, como vimos, é preciso enviar sua branch para o repositório remoto com o comando:

   ```bash
   git push origin minha-nova-branch
   ```

2. **Criar o Pull Request no GitHub** (ou na plataforma que você estiver usando):
   - Vá até o repositório no GitHub e você verá um botão sugerindo criar um Pull Request para a branch que acabou de enviar.
   - Clique em "Compare & pull request" (ou "Comparar e criar pull request").
   - Adicione um título e uma descrição que expliquem o que sua branch faz.
   - Clique em "Create pull request" (ou "Criar pull request") para enviar a solicitação.

3. **Aguarde a Revisão**: Depois de criar o PR, outros membros da equipe podem revisar, sugerir mudanças e até aprovar. Assim que estiver aprovado, alguém poderá mesclar (merge) o PR com a branch principal.

4. **Mesclar o PR**: Depois de revisado, o pull request pode ser mesclado com a branch principal pelo próprio autor ou por alguém autorizado no repositório. Basta clicar em "Merge pull request" no GitHub.

---

### Resumo dos Comandos

- Criar e mudar para uma nova branch:
  ```bash
  git checkout -b nome-da-branch
  ```

- Ver as branches existentes:
  ```bash
  git branch
  ```

- Fazer o push da branch para o repositório remoto:
  ```bash
  git push origin nome-da-branch
  ```

- Criar o Pull Request no GitHub ou plataforma similar.

Esses passos ajudam a manter o projeto organizado e permitem que cada pessoa trabalhe de forma independente, com mais segurança e colaboração.
