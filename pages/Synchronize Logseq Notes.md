## How to sync after configuring a branch upstream this repository?
- Execute uma linha de cada vez: 
  Navegue mudando o diretório até Pretty Notes `cd Documentos/Pretty\ Notes/`. Mandar arquivos para *staging* com `git add .` . Manda de *staging* para o repositório local `git commit -m ""`, mais precisamente para o histórico de commits, conhecido como o *repositório Git*. Verifica o status atual do repositório local `git status`. Enviar as alterações feitas no repositório local para o repositório remoto `git push`. 
  ```bash
  cd ~/Documentos/Pretty\ Notes/
  git add .
  git commit -m ""
  git status
  git push
  ```
-
- ## How to synchronize Logseq notes with GitHub for the first time?
	- [**logseq**]Desmarque a opção *`Ativar confirmação automática do Git`* o mesmo que *`Enable Git auto commit`*
	-
	- [**shell**] Vá até a pasta do Logseq `cd logseq/path`
		- **Caso exista um arquivo .git**: Exclua o arquivo .git com `rm .git`, antes de iniciar o repositório
	- Inicie o Repositório `git init`
	- Adicione *tracked files* com alterações e arquivos novos à área de *Staging*, `git add .`, o que também marca arquivos deletados para a remoção no próximo commit.
	- Verifique o que está em *Staging* `git status`
		- **Caso não haja credenciais**: Adicione credenciais Globais `it config --global user.email "you@example.com"` e ` git config --global user.name "Your Name"`
	- Dê o primeiro *commit* `git commit -m "init"`
	- Verifique os *logs* dos *commits* (registros das alterações), `git log`
		- **Caso não esteja instalado**: Instale o `gh` com `sudo apt install gh` e senha
	-
	- [**logseq**] Marcar *`Enable Git auto commit`*, definir o tempo para o auto commit (em segundos) e *`Git commit on window close`*, para ativar commmit automático, além de ativar commit ao fechar janela.
	-
	- [**shell**] Crie um repositório público no GitHub (remoto) `gh repo create <repository> --public`
		- **Caso tenha criado o repositório local primeiro e queira vinculá-lo a um repositório remoto criado manualmente no GitHub**: Conecte o repositório remoto (chamado `origin`) ao seu repositório Git local, associando-o ao URL especificado `git remote add origin https://github.com/<user>/<repo>.git`. Isso permite que você sincronize suas alterações locais com o repositório remoto no GitHub.
		  id:: 67dbbac5-9d2d-453b-80a5-e087be599fa4
		- **Porém**, normalmente o `gh repo create` já configura automaticamente o repositório remoto como `origin`, eliminando a necessidade de `git remote add origin`.
		  id:: 67dbbe4d-b681-4465-8033-9b82ddad793a
	- Abra o repositório para validar `open github.com/<user>/<repo>`
	- Valide a conexão entre os repositórios Local e Remoto, com o comando `git remote -v`, que deve retornar:
		- ```shell
		  > git remote -v
		  #return
		  origin  https://github.com/<user>/<repo>.git (fetch)
		  origin  https://github.com/<user>/<repo>.git (push)
		  ```
	- Renomeie a Branch atual para `main`, forçando a alteração mesmo que uma branch de mesmo nome já exista no repositório local, isso irá sobrescreve-la: `git branch -M main`.
		- **Caso o repositório remoto tenha sido configurado incorretamente, como com o URL errado, por exemplo. Caso o URL tenha mudado, seja por conta de o repositório ter sido movido ou renomeado**. Caso queira vincular o repositório local a um repositório remoto diferente.: deve remover `origin` para permitir uma configuração limpa, `git remote remove origin`
			- Havia configurado errado e
	- Com o comando `git push -u origin main` empurra os commits da branch `main` local para o repositório remoto configurado como `origin` e define `origin/main` como a branch upstream para facilitar futuros pushes e pulls.
	- Ao configurar uma *branch upstream*, ela facilita os próximos comandos de push e pull, de modo que não se faz mais necessário especificar o repositório (`origin`), tampouco a branch (`main`).
		- **Antes de  configurar uma branch upstream**: `git push origin main` ou `git pull origin main`
		- **Depois de  configurar uma branch upstream**: Apenas`git push` ou `git pull`
- Oque ocorre porque o Git sabe automaticamente qual *branch remota* está vinculada à sua *branch local*, permitindo uma comunicação mais fluida entre os repositórios. Isso torna seu fluxo de trabalho mais rápido.