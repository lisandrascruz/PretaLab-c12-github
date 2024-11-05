# Principais Comandos do Git e GitHub

Aqui está uma lista dos comandos mais importantes do Git e como usá-los no GitHub. Esses comandos permitem que você inicialize projetos, rastreie alterações no código, e faça upload para o GitHub, facilitando o desenvolvimento colaborativo.

#### 1. **Instalação do Git**
   Antes de tudo, você precisa instalar o Git. Baixe em [https://git-scm.com/downloads](https://git-scm.com/downloads) e siga as instruções para o seu sistema operacional.

#### 2. **Configurando o Git**
   Após a instalação, configure seu nome de usuário e e-mail, que aparecerão nas suas contribuições:
   ```bash
   git config --global user.name "SeuNome"
   git config --global user.email "seuemail@exemplo.com"
   ```

#### 3. **Verificando as configurações do git**
   Após as configurações serem atribuídas, elas podem ser verificadas a qualquer momento usando:
   ```bash
   git config --list
   ```

#### 4. **Clonando um Repositório**
   Para baixar um repositório existente do GitHub para o seu computador, use o `git clone` seguido da URL do repositório:
   ```bash
   git clone https://github.com/usuario/repositorio.git
   ```

#### 5. **Adicionando Mudanças**
   Depois de fazer alterações em seus arquivos, você precisa "adicioná-los" ao seu próximo commit. Use `git add` para isso:
   ```bash
   git add nome_do_arquivo    # Adiciona um arquivo específico
   git add .                  # Adiciona todos os arquivos modificados
   ```

#### 6. **Reservando alterações**
   O git stash é um comando do Git que permite salvar temporariamente as alterações no seu ambiente de trabalho (os arquivos que estão modificados ou não commitados) sem precisar fazer um commit.
   ```bash
   git stash        # armazena as mudanças
   git stash pop    # trás de volta para o código as mudanças anteriormente armazenadas
   ```

#### 7. **Criando um Commit**
   Para salvar as mudanças no repositório local, você cria um "commit" com uma mensagem descritiva sobre as alterações feitas:
   ```bash
   git commit -m "Mensagem descrevendo as alterações"
   ```

#### 8. **Enviando para o GitHub (Push)**
   Envie as alterações do seu repositório local para o repositório remoto no GitHub com `git push`:
   ```bash
   git push origin main       # Envia as mudanças para a branch 'main' no GitHub
   ```

#### 9. **Atualizando o Repositório Local (Pull)**
   Para sincronizar seu repositório local com as mudanças feitas por outras pessoas no repositório do GitHub, use `git pull`:
   ```bash
   git pull origin main
   ```

#### 10. **Verificando o Status**
   O comando `git status` exibe quais arquivos foram alterados, adicionados ou ainda não foram commitados, permitindo que você veja o que está acontecendo no repositório:
   ```bash
   git status
   ```

#### 11. **Verificando o Histórico de Commits**
   Use `git log` para visualizar o histórico de commits e ver as mudanças feitas ao longo do tempo:
   ```bash
   git log
   ```
