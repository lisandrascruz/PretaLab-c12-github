# Criando meu primeiro repositório

O Repositório é um local onde os arquivos de um projeto, incluindo o histórico de suas alterações, são armazenados e gerenciados utilizando o sistema de controle de versão Git. Ele permite que os usuários colaborem, façam alterações, rastreie mudanças e mantenha a integridade dos arquivos do projeto.

1. Acesse o seu github e façá login
2. Na página inicial, no canto superior direito, clique em `+` e escolha a opção `Novo repositório`
3. Dê um nome ao seu repositório, defina se será publico ou privado e por fim, clique em `Criar repositório` para finalizar a criação

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

#### 6. **Removendo Mudanças**
   Depois de adicionar, preparando seus arquivos para commit, você pode precisar "removê-los". Use `git reset` para isso:
   ```bash
   git reset nome_do_arquivo      # Remove um arquivo específico
   git reset .                    # Remove todos os arquivos adicionados
   ```

#### 7. **Criando um Commit**
   Para salvar as mudanças no repositório local, você cria um "commit" com uma mensagem descritiva sobre as alterações feitas:
   ```bash
   git commit -m "Mensagem descrevendo as alterações"
   ```
   conventional commits: feat, fix, style, docs, revert.

#### 8. **Removendo um commit local**
   Para apagar um commit feito enquanto está apenas localmente:
   ```bash
   git reset HEAD~2     # Reverte a posiçãso do commit local desejado `~`
   ```
   [leia mais sobre reverter commits](https://medium.com/@dieggocarrilho/como-desfazer-commit-local-e-remoto-a6409f0388d4)
   
#### 9. **Enviando para o GitHub (Push)**
   Envie as alterações do seu repositório local para o repositório remoto no GitHub com `git push`:
   ```bash
   git push origin main       # Envia as mudanças para a branch 'main' no GitHub
   ```

#### 10. **Atualizando o Repositório Local (Pull)**
   Para sincronizar seu repositório local com as mudanças feitas por outras pessoas no repositório do GitHub, use `git pull`:
   ```bash
   git pull origin main
   ```

#### 11. **Verificando o Status**
   O comando `git status` exibe quais arquivos foram alterados, adicionados ou ainda não foram commitados, permitindo que você veja o que está acontecendo no repositório:
   ```bash
   git status
   ```

#### 12. **Verificando o Histórico de Commits**
   Use `git log` para visualizar o histórico de commits e ver as mudanças feitas ao longo do tempo:
   ```bash
   git log
   ```

#### 13. **Reservando alterações**
   O git stash é um comando do Git que permite salvar temporariamente as alterações no seu ambiente de trabalho (os arquivos que estão modificados ou não commitados) sem precisar fazer um commit.
   ```bash
   git stash        # armazena as mudanças
   git stash pop    # trás de volta para o código as mudanças anteriormente armazenadas
   ```

