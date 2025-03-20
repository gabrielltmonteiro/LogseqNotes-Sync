## How to synchronize Logseq notes with GitHub for the first time?
title:: Synchronize Logseq Notes
	- [**logseq**]Desmarque a opção *`Ativar confirmação automática do Git`* o mesmo que *`Enable Git auto commit`*
	-
	- [**shell**] Vá até a pasta do Logseq `cd logseq/path`
		- **Caso exista um arquivo .git**: Exclua o arquivo .git com `rm .git`, antes de iniciar o repositório
	- Inicie o Repositório `git init`
	- Adicione *tracked files* e arquivos novos à área de *Stage*, `git add .`, o que também marca arquivos deletados para a remoção no próximo commit.
	- Verifique o que está em *Stage* `git status`
		- **Caso não haja credenciais**: Adicione credenciais Globais `it config --global user.email "you@example.com"` e ` git config --global user.name "Your Name"`
	- Dê o primeiro *commit* `git commit -m "init"`
	- Verifique os *logs* dos *commits* (registros das alterações), `git log`
		- **Caso não esteja instalado**: Instale o `gh` com `sudo apt install` e senha
	-
	- [**logseq**] Marcar *`Enable Git auto commit`*, definir o tempo para o auto commit (em segundos) e *`Git commit on window close`*, para ativar commmit automático, além de ativar commit ao fechar janela.
	-
	- [**shell**] Crie o repositório no GitHub (remoto) `gh repo create <user>/<LogseqNotesSync> --public`
		- Abra o repositório para validar `open github.com/<user>/<repo> &`
	- Conecte o repositório remoto (chamado `origin`) ao seu repositório Git local, associando-o ao URL especificado `git remote add origin https://github.com/<user>/<repo>.git`. Isso permite que você sincronize suas alterações locais com o repositório remoto no GitHub.
		- Valide a conexão entre os repositórios Local e Remoto, com o comando `git remote -v`, que deve retornar
			- ```shell
			  >
			  #return
			  origin  https://github.com/<user>/<repo>.git (fetch)
			  origin  https://github.com/<user>/<repo>.git (push)
			  ```
	- Renomeie a branch atual para `main`, forçando a alteração mesmo que uma branch de mesmo nome, também chamada `main`, já exista no repositório local, sobrescrevendo-a: `git branch -M main`.
	- Com o comando `git push -u origin main` empurra os commits da branch `main` local para o repositório remoto configurado como `origin` e define `origin/main` como a branch upstream para facilitar futuros pushes e pulls.
	- Ao configurar uma branch upstream, ela facilita os próximos comandos de push e pull, de modo que não se faz mais necessário especificar o repositório (`origin`), tampouco a branch (`main`).
		- **Antes de  configurar uma branch upstream**: `git push origin main` ou `git pull origin main`
		- **Depois de  configurar uma branch upstream**: Apenas`git push` ou `git pull`
- Oque ocorre porque o Git sabe automaticamente qual *branch remota* está vinculada à sua *branch local*, permitindo uma comunicação mais fluida entre os repositórios. Isso torna seu fluxo de trabalho mais rápido.
-
- ## How to sync after configuring a branch upstream this repository?
-
-