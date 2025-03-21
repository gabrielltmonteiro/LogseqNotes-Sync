# Bismuth Produtivo
collapsed:: true
	- Para utilizar o **Bismuth** de forma produtiva, o ideal é dominar os comandos mais frequentemente usados para gerenciar janelas e ajustar layouts. Aqui estão os principais:
	- ### **Gerenciamento da Área Master**
	- **Push Activate Window to Master Area**: Move a janela ativa para a área master, destacando-a como principal.
	- **Increase/Decrease Master Area Size**: Aumenta ou reduz o tamanho da área master.
	- **Increase/Decrease Master Area Window Count**: Ajusta o número de janelas simultâneas na área master.
	- ### **Navegação Entre Janelas**
	- **Focus Next/Previous Window**: Alterna entre as janelas na ordem do layout.
	- **Focus Left/Right/Upper/Bottom Window**: Move o foco para janelas específicas com base em sua posição no layout.
	- ### **Reorganização de Janelas**
	- **Move Window Right/Left/Up/Down**: Reposiciona a janela atual no layout.
	- **Move Window to the Next/Previous Position**: Altera a posição da janela na sequência do layout.
	- ### **Ajuste de Tamanho**
	- **Increase/Decrease Window Width**: Ajusta a largura da janela selecionada.
	- **Increase/Decrease Window Height**: Ajusta a altura da janela selecionada.
	- ### **Troca e Alternância de Layouts**
	- **Switch to the Next/Previous Layout**: Alterna entre os layouts disponíveis.
	- **Toggle Tile Layout**: Ativa ou desativa o layout de mosaico.
	- **Toggle Monocle Layout**: Alterna para o layout de tela cheia (uma janela visível por vez).
	- **Toggle Floating Layout**: Habilita ou desabilita o layout flutuante, permitindo maior liberdade de movimento.
	- ### **Outros Comandos Úteis**
	- **Rotate/Rotate (Reverse)**: Rotaciona as janelas no layout no sentido horário ou anti-horário.
	- **Toggle Activate Window Floating**: Alterna a janela ativa para o modo flutuante.
	- **Toggle Quarter, Spiral, Spread, Stair, or Three Column Layout**: Testa diferentes layouts para atender melhor às suas necessidades.
	- ### **Dicas para Ser Mais Produtivo**
	- Configure **atalhos de teclado** intuitivos para os comandos que você usa com mais frequência.
	- Combine layouts diferentes dependendo do fluxo de trabalho (exemplo: Monocle para foco ou Three Column para multitarefas).
	- Experimente os comandos de rotação (Rotate) e ajuste de área master para otimizar espaço em tempo real.
	  
	  Com esses comandos, você pode transformar o gerenciamento de janelas em algo rápido e eficiente! Quer ajuda com algo específico? 😊
- # git remote add origin
  collapsed:: true
	- O comando que você mencionou está quase pronto para uso! Ele é usado para adicionar um repositório remoto chamado `origin` ao repositório Git local, associando-o ao URL especificado. Aqui está como você deve personalizá-lo:
	- 1. **Substitua `<user>`** pelo nome do seu usuário ou organização do GitHub.
	  2. **Substitua `<repository>`** pelo nome do repositório que você criou no GitHub.
	- Por exemplo, se o seu nome de usuário for `gabrielltmonteiro` e o nome do repositório for `LogseqNotesSync`, o comando será:
	  ```bash
	  git remote add origin https://github.com/gabrielltmonteiro/LogseqNotesSync.git
	  ```
	- Depois de adicionar o repositório remoto, você pode confirmar a configuração com:
	  ```bash
	  git remote -v
	  ```
	- A partir daí, estará pronto para enviar (`push`) suas alterações para o repositório remoto:
	  ```bash
	  git push -u origin main
	  ```
	- Se precisar de mais ajuda, é só me chamar! 😊
	-
	-
	- **Resumo**
	- De forma resumida, o comando `git remote add origin https://github.com/<user>/<repository>.git` adiciona um repositório remoto (chamado "origin") ao seu repositório Git local, associando-o ao URL especificado. Isso permite que você sincronize suas alterações locais com o repositório remoto no GitHub. 🚀
	-
	-
	- O comando `git remote add origin https://github.com/<user>/<repository>.git` é usado para **configurar um repositório remoto** no Git. Vamos detalhar:
	  
	  1. **`git remote add`**: Este comando adiciona uma nova conexão remota ao seu repositório Git local.
	  2. **`origin`**: O nome "origin" é convencionalmente usado como o apelido para o repositório remoto principal. Você pode usar outro nome, mas "origin" é o padrão.
	  3. **`https://github.com/<user>/<repository>.git`**: O URL representa o endereço do repositório remoto. Substitua `<user>` pelo nome do usuário ou organização no GitHub e `<repository>` pelo nome do repositório.
	  
	  Quando você executa esse comando, o Git associa o repositório remoto especificado ao seu repositório local. Depois disso, você pode:
	- **Enviar alterações ao remoto (push)**: Por exemplo, `git push origin main`.
	- **Buscar atualizações do remoto (fetch)**: Por exemplo, `git fetch origin`.
	- **Clonar, sincronizar, ou realizar outras operações Git relacionadas ao repositório remoto.**
	  
	  Se precisar de mais explicações ou ajuda com outro comando, me avise! 😊
- # git branch -M main
  collapsed:: true
	- O comando `git branch -M main` renomeia a branch atual para `main` e faz isso de forma forçada, garantindo que mesmo se já existir uma branch chamada `main`, ela será sobrescrita. Aqui está o que ele faz de forma resumida:
	- 1. **Renomeia**: Altera o nome da branch atual para `main`.
	  2. **Força a mudança**: Caso já exista uma branch chamada `main`, ela será substituída.
	- Isso é útil em situações em que você quer alinhar o nome da branch principal com o padrão moderno de nomenclatura (`main` em vez de `master`). 🚀
	-
	- Exatamente! O comando `git branch -M main` **renomeia a branch atual para **`main` e faz isso de forma **forçada**, sobrescrevendo qualquer branch chamada `main` que já exista no repositório local. 🚀
	- Se precisar de mais explicações ou exemplos, é só avisar! 😊
	-
	- Se a branch atual já estiver com o nome **diferente de `main`**, o comando `git branch -M main` **renomeará a branch atual para `main`** sem problemas. No entanto, se **já existir uma branch chamada `main` no repositório local**, esse comando irá forçar a substituição dela pela branch atual.
	  
	  Ou seja:
	- O comando **ignora a existência de outra branch `main`** no repositório local e sobrescreve o nome dela.
	- A branch que antes era chamada de `main` será descartada localmente, e a branch atual assumirá o nome `main`.
	  
	  Portanto, é importante usar o comando com cuidado, especialmente se houver informações importantes na branch `main` já existente. Para verificar suas branches antes de renomear, você pode usar:
	  ```bash
	  git branch
	  ``` 
	  
	  Se precisar de mais dicas, é só chamar! 😊
- # git push -u origin main
  collapsed:: true
	- O comando envia os commits da branch `main` local para o repositório remoto configurado como `origin`. Além disso, define `origin/main` como a branch upstream para facilitar futuros pushes e pulls.
	-
	- O comando `git push -u origin main` **empurra da branch local **`main`** para a remota** e define `origin/main` como a branch upstream, facilitando futuros pushes e pulls. É importante substituir "branch" pelo nome específico, neste caso, `main`. 😊
	-
- # branch upstream
  collapsed:: true
	- ma **branch upstream** é a branch remota à qual uma branch local está conectada. Ela é usada como referência para sincronização entre o repositório local e o remoto. Quando uma branch local tem uma upstream configurada, comandos como `git pull` e `git push` podem ser usados diretamente, sem precisar especificar o nome do repositório ou branch.
	  
	  Por exemplo:
	- No comando `git push -u origin main`, a branch local `main` é vinculada à branch `origin/main` no remoto como upstream, facilitando futuros comandos. 🚀
	-
	-
	-
	- Quando uma branch upstream é configurada com `git push -u origin main`, ela facilita os próximos comandos de `push` e `pull` porque:
	- **Simplificação dos comandos**: Você não precisa mais especificar o repositório (`origin`) nem a branch (`main`) nos próximos comandos. Por exemplo:
		- **Antes**: `git push origin main` ou `git pull origin main`.
		- **Depois**: Apenas `git push` ou `git pull`.
	- **Sincronização direta**: O Git sabe automaticamente qual branch remota está vinculada à sua branch local, permitindo uma comunicação mais fluida entre os repositórios local e remoto.
	  
	  Isso torna seu fluxo de trabalho mais rápido e eficiente! 🚀
	- Isso ocorre **depois de configurar uma branch upstream**. Quando você executa o comando `git
	-
	- push -u origin main`, além de enviar os commits da branch `main` para o repositório remoto, ele define a branch `origin/main` como a upstream. Esse vínculo é o que permite simplificar futuros comandos de `push` e `pull`, sem precisar especificar o repositório ou a branch novamente. Portanto, a simplificação só acontece após essa configuração. 🚀
- # git remote remove origin
  collapsed:: true
	- O comando `git remote remove origin` remove a configuração remota chamada **`origin`** do repositório local. Isso significa que o link entre seu repositório local e o repositório remoto (geralmente no GitHub ou similar) será desfeito.
	- Após executá-lo, o repositório local não terá mais referência ao remoto `origin`, e você pode verificar isso com:
	  ```bash
	  git remote -v
	  ```
	- Este comando não afeta o repositório remoto ou seus dados, apenas a conexão no repositório local. Se precisar adicioná-lo novamente, é só configurar com `git remote add origin <URL>`. 🚀
	-
	-
	-
	- O comando `git remote remove origin` é necessário em situações como:
	- 1. **Reconfiguração do repositório remoto**: Quando o URL remoto mudou (por exemplo, o repositório foi movido ou renomeado), você pode remover o antigo `origin` para adicionar o novo.
	   ```bash
	   git remote add origin <novo-URL>
	   ```
	- 2. **Troca do repositório remoto**: Caso queira vincular o repositório local a um repositório remoto diferente.
	- 3. **Correção de configurações erradas**: Se o repositório remoto foi configurado incorretamente (URL errado, por exemplo), remover `origin` permite uma configuração limpa.
	- 4. **Desvincular do remoto**: Se você não precisa mais de um repositório remoto associado, o comando remove a referência.
	- Se precisar de mais detalhes sobre como reconfigurar ou corrigir as referências remotas, é só avisar! 😊
-
- Terminal
- ```Bash
  
  gabe/Documentos/Pretty Notes 
  ❯ git log
  commit 706aed7a80a7f028444378a0e4ff101712d9e458 (HEAD -> master)
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 14:31:09 2025 -0300
  
      Auto saved by Logseq
  
  commit 43268b54f529ac37a75502a49482558d42c62c6b
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 14:23:56 2025 -0300
  
      init
  
  gabe/Documentos/Pretty Notes 
  ❯ git diff
  
  gabe/Documentos/Pretty Notes 
  ❯ git diff 43268b54f529ac37a75502a49482558d42c62c6b
  diff --git a/pages/Test.md b/pages/Test.md
  new file mode 100644
  index 0000000..6b5dba0
  --- /dev/null
  +++ b/pages/Test.md
  @@ -0,0 +1 @@
  +- Test
  \ No newline at end of file
  
  gabe/Documentos/Pretty Notes 
  ❯ git diff 43268b54f529ac37a75502a49482558d42c62c6b
  diff --git a/pages/Test.md b/pages/Test.md
  new file mode 100644
  index 0000000..07821fb
  --- /dev/null
  +++ b/pages/Test.md
  @@ -0,0 +1,2 @@
  +- Test
  +       - Changing
  \ No newline at end of file
  
  gabe/Documentos/Pretty Notes 
  ❯ sudo apt install gh
  [sudo] senha para gabe: 
  Lendo listas de pacotes... Pronto
  Construindo árvore de dependências... Pronto
  Lendo informação de estado... Pronto        
  gh já é a versão mais recente (2.4.0+dfsg1-2).
  0 pacotes atualizados, 0 pacotes novos instalados, 0 a serem removidos e 1 não atualizados.
  
  gabe/Documentos/Pretty Notes took 3s 
  ❯ gh repo create gabrielltmonteiro/logsync    
  `--public`, `--private`, or `--internal` required when not running interactively
  
  Usage:  gh repo create [<name>] [flags]
  
  Flags:
    -c, --clone                 Clone the new repository to the current directory
    -d, --description string    Description of the repository
        --disable-issues        Disable issues in the new repository
        --disable-wiki          Disable wiki in the new repository
    -g, --gitignore string      Specify a gitignore template for the repository
    -h, --homepage URL          Repository home page URL
        --internal              Make the new repository internal
    -l, --license string        Specify an Open Source License for the repository
        --private               Make the new repository private
        --public                Make the new repository public
        --push                  Push local commits to the new repository
    -r, --remote string         Specify remote name for the new repository
    -s, --source string         Specify path to local repository to use as source
    -t, --team name             The name of the organization team to be granted access
    -p, --template repository   Make the new repository based on a template repository
    
  
  gabe/Documentos/Pretty Notes 
  ❯ gh create repo gabrielltmonteiro/logsync    
  unknown command "create" for "gh"
  
  Usage:  gh <command> <subcommand> [flags]
  
  Available commands:
    actions
    alias
    api
    auth
    browse
    codespace
    completion
    config
    extension
    gist
    gpg-key
    help
    issue
    pr
    release
    repo
    run
    secret
    ssh-key
    workflow
  
  
  gabe/Documentos/Pretty Notes 
  ❯ gh repo create gabrielltmonteiro/logsync    
  `--public`, `--private`, or `--internal` required when not running interactively
  
  Usage:  gh repo create [<name>] [flags]
  
  Flags:
    -c, --clone                 Clone the new repository to the current directory
    -d, --description string    Description of the repository
        --disable-issues        Disable issues in the new repository
        --disable-wiki          Disable wiki in the new repository
    -g, --gitignore string      Specify a gitignore template for the repository
    -h, --homepage URL          Repository home page URL
        --internal              Make the new repository internal
    -l, --license string        Specify an Open Source License for the repository
        --private               Make the new repository private
        --public                Make the new repository public
        --push                  Push local commits to the new repository
    -r, --remote string         Specify remote name for the new repository
    -s, --source string         Specify path to local repository to use as source
    -t, --team name             The name of the organization team to be granted access
    -p, --template repository   Make the new repository based on a template repository
    
  
  gabe/Documentos/Pretty Notes 
  ❯ gh repo create gabrielltmonteiro/LogseqNotesSync --public
  ✓ Created repository gabrielltmonteiro/LogseqNotesSync on GitHub
  
  gabe/Documentos/Pretty Notes 
  ❯  gabrielltmonteiro/LogseqNotesSync
  bash: gabrielltmonteiro/LogseqNotesSync: Arquivo ou diretório inexistente
  
  gabe/Documentos/Pretty Notes 
  ❯ 
  
  gabe/Documentos/Pretty Notes 
  ❯ open  gabrielltmonteiro/LogseqNotesSync
  kf.service.services: The desktop entry file "/usr/share/applications/org.gnome.ChromeGnomeShell.desktop" has Type= "Application" but no Exec line
  kf.service.sycoca: Invalid Service :  "/usr/share/applications/org.gnome.ChromeGnomeShell.desktop"
  kf.service.services: The desktop entry file "/home/gabe/.local/share/applications/emacs-term.desktop" has Type= "Application" but no Exec line
  kf.service.sycoca: Invalid Service :  "/home/gabe/.local/share/applications/emacs-term.desktop"
  kf.service.services: The desktop entry file "/home/gabe/.local/share/applications/powershell_powershell.desktop" has Type= "Application" but no Exec line
  kf.service.sycoca: Invalid Service :  "/home/gabe/.local/share/applications/powershell_powershell.desktop"
  kf.config.core: "KConfigIni: In file /opt/zotero/zotero.desktop, line 3: " "Invalid escape sequence \"\\/\"."
  kf.config.core: "KConfigIni: In file /opt/zotero/zotero.desktop, line 3: " "Invalid escape sequence \"\\/\"."
  kf.service.sycoca: The menu spec file ( "" ) contains a Layout or DefaultLayout tag without the mandatory Merge tag inside. Please fix it.
  kf.service.sycoca: The menu spec file ( "" ) contains a Layout or DefaultLayout tag without the mandatory Merge tag inside. Please fix it.
  kf.service.sycoca: The menu spec file ( "" ) contains a Layout or DefaultLayout tag without the mandatory Merge tag inside. Please fix it.
  kf.service.sycoca: The menu spec file ( "" ) contains a Layout or DefaultLayout tag without the mandatory Merge tag inside. Please fix it.
  Icon theme "gnome" not found.
  Abrindo em uma sessão de navegador existente.
  
  gabe/Documentos/Pretty Notes 
  ❯ open  github.com/LogseqNotesSync
  Icon theme "gnome" not found.
  Abrindo em uma sessão de navegador existente.
  
  gabe/Documentos/Pretty Notes 
  ❯ gh repo edit LogseqNotesSync --name "LogseqNotes-Synchronize"
  unknown flag: --name
  
  Usage:  gh repo edit [<repository>] [flags]
  
  Flags:
        --add-topic strings        Add repository topic
        --allow-forking            Allow forking of an organization repository
        --default-branch name      Set the default branch name for the repository
        --delete-branch-on-merge   Delete head branch when pull requests are merged
    -d, --description string       Description of the repository
        --enable-auto-merge        Enable auto-merge functionality
        --enable-issues            Enable issues in the repository
        --enable-merge-commit      Enable merging pull requests via merge commit
        --enable-projects          Enable projects in the repository
        --enable-rebase-merge      Enable merging pull requests via rebase
        --enable-squash-merge      Enable merging pull requests via squashed commit
        --enable-wiki              Enable wiki in the repository
    -h, --homepage URL             Repository home page URL
        --remove-topic strings     Remove repository topic
        --template                 Make the repository available as a template repository
        --visibility string        Change the visibility of the repository to {public,private,internal}
    
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote add origin gabrielltmonteiro/LogseqNotesSync
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote add origin https://github.com/gabrielltmonteiro/LogseqNotesSync.git
  error: remote origin already exists.
  
  gabe/Documentos/Pretty Notes 
  ❯ git branch -M main
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -list
  error: unknown switch `l'
  uso: git remote [-v | --verbose]
     ou: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
     ou: git remote rename <old> <new>
     ou: git remote remove <name>
     ou: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
     ou: git remote [-v | --verbose] show [-n] <name>
     ou: git remote prune [-n | --dry-run] <name>
     ou: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
     ou: git remote set-branches [--add] <name> <branch>...
     ou: git remote get-url [--push] [--all] <name>
     ou: git remote set-url [--push] <name> <newurl> [<oldurl>]
     ou: git remote set-url --add <name> <newurl>
     ou: git remote set-url --delete <name> <url>
  
      -v, --verbose         be verbose; must be placed before a subcommand
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -l
  error: unknown switch `l'
  uso: git remote [-v | --verbose]
     ou: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
     ou: git remote rename <old> <new>
     ou: git remote remove <name>
     ou: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
     ou: git remote [-v | --verbose] show [-n] <name>
     ou: git remote prune [-n | --dry-run] <name>
     ou: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
     ou: git remote set-branches [--add] <name> <branch>...
     ou: git remote get-url [--push] [--all] <name>
     ou: git remote set-url [--push] <name> <newurl> [<oldurl>]
     ou: git remote set-url --add <name> <newurl>
     ou: git remote set-url --delete <name> <url>
  
      -v, --verbose         be verbose; must be placed before a subcommand
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git origin -list
  git: 'origin' não é um comando git. Veja 'git --help'.
  
  gabe/Documentos/Pretty Notes 
  ❯ git origin --list
  git: 'origin' não é um comando git. Veja 'git --help'.
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  gabrielltmonteiro/LogseqNotesSync (fetch)
  origin  gabrielltmonteiro/LogseqNotesSync (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git branch -M main
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  gabrielltmonteiro/LogseqNotesSync (fetch)
  origin  gabrielltmonteiro/LogseqNotesSync (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u origin main
  fatal: 'gabrielltmonteiro/LogseqNotesSync' does not appear to be a git repository
  fatal: Could not read from remote repository.
  
  Please make sure you have the correct access rights
  and the repository exists.
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u origin
  fatal: The current branch main has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin main
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u origin master
  error: src refspec master does not match any
  error: failed to push some refs to 'gabrielltmonteiro/LogseqNotesSync'
  
  gabe/Documentos/Pretty Notes 
  ❯ git push origin master
  error: src refspec master does not match any
  error: failed to push some refs to 'gabrielltmonteiro/LogseqNotesSync'
  
  gabe/Documentos/Pretty Notes 
  ❯ git push origin
  fatal: The current branch main has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin main
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git push --set-upstream origin main
  fatal: 'gabrielltmonteiro/LogseqNotesSync' does not appear to be a git repository
  fatal: Could not read from remote repository.
  
  Please make sure you have the correct access rights
  and the repository exists.
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  gabrielltmonteiro/LogseqNotesSync (fetch)
  origin  gabrielltmonteiro/LogseqNotesSync (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git branch -M main
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  gabrielltmonteiro/LogseqNotesSync (fetch)
  origin  gabrielltmonteiro/LogseqNotesSync (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u -u origin
  fatal: The current branch main has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin main
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u origin
  fatal: The current branch main has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin main
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git push origin
  fatal: The current branch main has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin main
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  gabrielltmonteiro/LogseqNotesSync (fetch)
  origin  gabrielltmonteiro/LogseqNotesSync (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote add origin https://github.com/gabrielltmonteiro/LogseqNotesSync.git
  error: remote origin already exists.
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote remove origin
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote remove origin
  error: No such remote: 'origin'
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote add origin https://github.com/gabrielltmonteiro/LogseqNotesSync.git
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  https://github.com/gabrielltmonteiro/LogseqNotesSync.git (fetch)
  origin  https://github.com/gabrielltmonteiro/LogseqNotesSync.git (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git branch -M main
  
  gabe/Documentos/Pretty Notes 
  ❯ git remote -v
  origin  https://github.com/gabrielltmonteiro/LogseqNotesSync.git (fetch)
  origin  https://github.com/gabrielltmonteiro/LogseqNotesSync.git (push)
  
  gabe/Documentos/Pretty Notes 
  ❯ git push -u origin main
  Enumerating objects: 15, done.
  Counting objects: 100% (15/15), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (10/10), done.
  Writing objects: 100% (15/15), 6.09 KiB | 6.09 MiB/s, done.
  Total 15 (delta 1), reused 0 (delta 0), pack-reused 0
  remote: Resolving deltas: 100% (1/1), done.
  To https://github.com/gabrielltmonteiro/LogseqNotesSync.git
   * [new branch]      main -> main
  Branch 'main' set up to track remote branch 'main' from 'origin'.
  
  gabe/Documentos/Pretty Notes 
  ❯ gh repo edit LogseqNotesSync --name "LogseqNotes-Sync"
  unknown flag: --name
  
  Usage:  gh repo edit [<repository>] [flags]
  
  Flags:
        --add-topic strings        Add repository topic
        --allow-forking            Allow forking of an organization repository
        --default-branch name      Set the default branch name for the repository
        --delete-branch-on-merge   Delete head branch when pull requests are merged
    -d, --description string       Description of the repository
        --enable-auto-merge        Enable auto-merge functionality
        --enable-issues            Enable issues in the repository
        --enable-merge-commit      Enable merging pull requests via merge commit
        --enable-projects          Enable projects in the repository
        --enable-rebase-merge      Enable merging pull requests via rebase
        --enable-squash-merge      Enable merging pull requests via squashed commit
        --enable-wiki              Enable wiki in the repository
    -h, --homepage URL             Repository home page URL
        --remove-topic strings     Remove repository topic
        --template                 Make the repository available as a template repository
        --visibility string        Change the visibility of the repository to {public,private,internal}
    
  
  gabe/Documentos/Pretty Notes 
  ❯ gh repo edit "LogseqNotesSync" --name "LogseqNotes-Sync"
  unknown flag: --name
  
  Usage:  gh repo edit [<repository>] [flags]
  
  Flags:
        --add-topic strings        Add repository topic
        --allow-forking            Allow forking of an organization repository
        --default-branch name      Set the default branch name for the repository
        --delete-branch-on-merge   Delete head branch when pull requests are merged
    -d, --description string       Description of the repository
        --enable-auto-merge        Enable auto-merge functionality
        --enable-issues            Enable issues in the repository
        --enable-merge-commit      Enable merging pull requests via merge commit
        --enable-projects          Enable projects in the repository
        --enable-rebase-merge      Enable merging pull requests via rebase
        --enable-squash-merge      Enable merging pull requests via squashed commit
        --enable-wiki              Enable wiki in the repository
    -h, --homepage URL             Repository home page URL
        --remove-topic strings     Remove repository topic
        --template                 Make the repository available as a template repository
        --visibility string        Change the visibility of the repository to {public,private,internal}
    
  
  gabe/Documentos/Pretty Notes 
  ❯ git status
  No ramo main
  Seu ramo está à frente de 'origin/main' por 1 submissão.
    (use "git push" to publish your local commits)
  
  nothing to commit, working tree clean
  
  gabe/Documentos/Pretty Notes 
  ❯ gh status
  unknown command "status" for "gh"
  
  Usage:  gh <command> <subcommand> [flags]
  
  Available commands:
    actions
    alias
    api
    auth
    browse
    codespace
    completion
    config
    extension
    gist
    gpg-key
    help
    issue
    pr
    release
    repo
    run
    secret
    ssh-key
    workflow
  
  
  gabe/Documentos/Pretty Notes 
  ❯ git status
  No ramo main
  Seu ramo está à frente de 'origin/main' por 1 submissão.
    (use "git push" to publish your local commits)
  
  nothing to commit, working tree clean
  
  gabe/Documentos/Pretty Notes 
  ❯ git push
  Enumerating objects: 7, done.
  Counting objects: 100% (7/7), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (3/3), done.
  Writing objects: 100% (4/4), 392 bytes | 392.00 KiB/s, done.
  Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
  remote: This repository moved. Please use the new location:
  remote:   https://github.com/gabrielltmonteiro/LogseqNotes-Sync.git
  To https://github.com/gabrielltmonteiro/LogseqNotesSync.git
     2c71a67..028a1de  main -> main
  
  gabe/Documentos/Pretty Notes 
  ❯ ^C
  
  gabe/Documentos/Pretty Notes 
  ❯ git push
  Enumerating objects: 54, done.
  Counting objects: 100% (54/54), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (45/45), done.
  Writing objects: 100% (52/52), 5.57 KiB | 1.86 MiB/s, done.
  Total 52 (delta 16), reused 0 (delta 0), pack-reused 0
  remote: Resolving deltas: 100% (16/16), done.
  remote: This repository moved. Please use the new location:
  remote:   https://github.com/gabrielltmonteiro/LogseqNotes-Sync.git
  To https://github.com/gabrielltmonteiro/LogseqNotesSync.git
     028a1de..b370998  main -> main
  
  gabe/Documentos/Pretty Notes 
  ❯ git diff
  diff --git a/pages/How do I synchronize Logseq notes with GitHub for the first time%3F.md b/pages/How do I synchronize Logseq notes with GitHub for the first time%3F.md
  index 81f7a60..b9e35d0 100644
  --- a/pages/How do I synchronize Logseq notes with GitHub for the first time%3F.md  
  +++ b/pages/How do I synchronize Logseq notes with GitHub for the first time%3F.md  
  @@ -16,13 +16,14 @@
          - Abra o repositório para validar `open github.com/<user>/<repo> &`
   - Conecte o repositório remoto (chamado `origin`) ao seu repositório Git local, associando-o ao URL especificado `git remote add origin https://github.com/<user>/<repo>.git`. Isso permite que você sincronize suas alterações locais com o repositório remoto no GitHub.
          - Valide a conexão entre os repositórios Local e Remoto, com o comando `git remote -v`, que deve retornar
  -               - origin  https://github.com/<user>/<repo>.git (fetch)
  -                 id:: 67db4a41-f143-4b8e-8ebe-b8387d485db5
  +               - ```shell
  +                 > gh repo create <user>/<LogseqNotesSync> --public
  +                 #return
  +                 origin  https://github.com/<user>/<repo>.git (fetch)
                    origin  https://github.com/<user>/<repo>.git (push)
  -- Renomeie a branch atual para `main`, forçando a alteração mesmo que uma branch chamada `main` já exista no repositório local, sobrescrevendo-a: `git branch -M main`.
  -- Envie os commits da branch `main` local para o repositório remoto configurado como `origin`. 
  -  `git push -u origin main`
  
  [1]+  Parado                  git diff
  
  gabe/Documentos/Pretty Notes took 5s 
  ✦ ❯ git status
  No ramo main
  Your branch is up to date with 'origin/main'.
  
  Changes not staged for commit:
    (utilize "git add <arquivo>..." para atualizar o que será submetido)
    (use "git restore <file>..." to discard changes in working directory)
          modified:   pages/How do I synchronize Logseq notes with GitHub for the first time%3F.md
  
  nenhuma modificação adicionada à submissão (utilize "git add" e/ou "git commit -a")
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git add .
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git commit -m "feat: note update"
  [main 35211c7] feat: note update
   1 file changed, 7 insertions(+), 6 deletions(-)
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git diff 35211c7
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git push
  Enumerating objects: 7, done.
  Counting objects: 100% (7/7), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (4/4), done.
  Writing objects: 100% (4/4), 565 bytes | 565.00 KiB/s, done.
  Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
  remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
  remote: This repository moved. Please use the new location:
  remote:   https://github.com/gabrielltmonteiro/LogseqNotes-Sync.git
  To https://github.com/gabrielltmonteiro/LogseqNotesSync.git
     b370998..35211c7  main -> main
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git branch -vv
  * main 35211c7 [origin/main] feat: note update
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git branch -v
  * main 35211c7 feat: note update
  
  gabe/Documentos/Pretty Notes 
  ✦ ❯ git log
  commit ff7534568d5cd95c6eb1d2acc514f917a4925785 (HEAD -> main)
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 23:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit b6db92cd12c6216342af2fba34d7d91416dc0834
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 22:49:18 2025 -0300
  
      Auto saved by Logseq
  
  commit 35211c7325ef0d622d267c6e83723bc6828c9d82 (origin/main)
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 22:18:05 2025 -0300
  
      feat: note update
  
  commit b3709981c53c648250ed06780c8c303457d5b033
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 20:51:32 2025 -0300
  
      Auto saved by Logseq
  
  commit ecaa778c8a7db3a09e4d112502a35aef67def04b
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 19:51:32 2025 -0300
  
  
  [2]+  Parado                  git log
  
  gabe/Documentos/Pretty Notes took 22s 
  ✦2 ❯ git push
  Enumerating objects: 12, done.
  Counting objects: 100% (12/12), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (10/10), done.
  Writing objects: 100% (10/10), 2.92 KiB | 2.92 MiB/s, done.
  Total 10 (delta 1), reused 0 (delta 0), pack-reused 0
  remote: Resolving deltas: 100% (1/1), done.
  remote: This repository moved. Please use the new location:
  remote:   https://github.com/gabrielltmonteiro/LogseqNotes-Sync.git
  To https://github.com/gabrielltmonteiro/LogseqNotesSync.git
     35211c7..ff75345  main -> main
  
  gabe/Documentos/Pretty Notes 
  ✦2 ❯ git log
  commit 1b99785c73ee6aff348476d8da645c89a71bd34e (HEAD -> ma
  commit 1b99785c73ee6aff348476d8da645c89a71bd34e (HEAD -> main)
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Thu Mar 20 03:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit 95ba48ccc7d3c29043de00a9165cf42c78559ef0
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Thu Mar 20 02:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit 64d64e03c403b4d64ea8be04f66edec2d8a7bad2 (origin/main)
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Thu Mar 20 02:23:04 2025 -0300
  
      Logseq Notes Update
  
  commit b59c0b57d6fe9eb78575ba4233c9614c5f9f9987
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Thu Mar 20 01:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit e1ee5b58fe9a40cfe2421d7c732fc43fae6ebbc5
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Thu Mar 20 00:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit ff7534568d5cd95c6eb1d2acc514f917a4925785
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 23:50:10 2025 -0300
  
      Auto saved by Logseq
  
  commit b6db92cd12c6216342af2fba34d7d91416dc0834
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 22:49:18 2025 -0300
  
      Auto saved by Logseq
  
  commit 35211c7325ef0d622d267c6e83723bc6828c9d82
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 22:18:05 2025 -0300
  
      feat: note update
  
  commit b3709981c53c648250ed06780c8c303457d5b033
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 20:51:32 2025 -0300
  
      Auto saved by Logseq
  
  commit ecaa778c8a7db3a09e4d112502a35aef67def04b
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 19:51:32 2025 -0300
  
      Auto saved by Logseq
  
  commit b10c819932afd0fae345f9b4eca68e8a3f7c9332
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 18:51:28 2025 -0300
  
      Auto saved by Logseq
  
  commit 230e87e63fe250c3977d75f324fba51559e09d3a
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 18:37:08 2025 -0300
  
      Auto saved by Logseq
  
  commit f6a99ae2c9a49d508eefd222877d08ab6f1f4232
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 17:37:08 2025 -0300
  
      Auto saved by Logseq
  
  commit f48bad8b28887d01b72f1be38ad109c98a4dcd03
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:34:28 2025 -0300
  
      Auto saved by Logseq
  
  commit 90bef8e6e362b1495b10bf7d255c3fb534fe0be5
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:34:18 2025 -0300
  
      Auto saved by Logseq
  
  commit 67e52e867d32adefd22eec08c89c0af51b4a8376
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:34:08 2025 -0300
  
      Auto saved by Logseq
  
  commit 339bd22e57434e3ab01be531281e169ba07155c9
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:33:58 2025 -0300
  
      Auto saved by Logseq
  
  commit 2c6d3e93047f339ffb1ef6a42853b97fc5d34a70
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:33:48 2025 -0300
  
      Auto saved by Logseq
  
  commit 231595cd0395664d20a54942f01ea7dea26537d4
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:33:38 2025 -0300
  
      Auto saved by Logseq
  
  commit 82afb2c25580be8fe3fac151ac11a39edd6afc5d
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:33:28 2025 -0300
  
      Auto saved by Logseq
  
  commit e83fc315d19d1e22415c7283465083b513955361
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:33:18 2025 -0300
  
      Auto saved by Logseq
  
  commit 028a1dec0a79bb2c4fdb919a3e9b0735f365ebcb
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 16:30:18 2025 -0300
  
      Auto saved by Logseq
  
  commit 2c71a673ea1ddb397ed990f3ea58efdc87ba7bc7
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 14:33:09 2025 -0300
  
      Auto saved by Logseq
  
  commit 706aed7a80a7f028444378a0e4ff101712d9e458
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 14:31:09 2025 -0300
  
      Auto saved by Logseq
  
  commit 43268b54f529ac37a75502a49482558d42c62c6b
  Author: gabrielltmonteiro <gabrielltmonteiro@hotmail.com>
  Date:   Wed Mar 19 14:23:56 2025 -0300
  
      init
  
  
  gabe/Documentos/Pretty Notes took 32s 
  ✦2 ❯ 
  ```