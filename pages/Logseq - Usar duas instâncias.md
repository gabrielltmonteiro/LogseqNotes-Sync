- **Logseq** foi originalmente instalado em `Flapak`
- Para usa duas instâncias verifique se as duas versões, `snap` e `flatpak` , estão instaladas:
	- ```bash
	  snap list #busque por Name=logseq
	  flatpak list #busque por Nome=Logseq, Inc.
	  ```
- **IF**: Logseq == **! Instalado em flatpak** OR **! instalado em snap**
  collapsed:: true
	- Instale e verifique se realmente está instalado
		- **IF**: Logseq **! Instalado em flatpak**
			- `flatpak install flathub com.logseq.Logseq`
			- Ou instale pela **Store**.
		- **ELIF**: Logseq **! instalado em snap**
			- `sudo snap install logseq`
- **ELIF**: Logseq == **Instalado em flatpak** AND **instalado em snap**
	- **Alternativa 1 (CLI)**: com o terminal **Bash** abrir ambos os Logseq em segundo plano `&` e impedindo que os processos sejam encerrados ao fechar o terminal.
		- ```bash
		  nohup snap run logseq &
		  nohup flatpak run com.logseq.Logseq &
		  ```
		- ![Screenshot_20250321_202749.png](../assets/Screenshot_20250321_202749_1742599731056_0.png)
		- #### **Equivalente a rodar cada um normalmente e definir posteriormente:**
		  collapsed:: true
			- Um de cada vez!
			- **Rodar logseq em `snap`**
			  ```Bash
			  snap run logseq
			  ```
			  **`CTRL+Z`**
			  Colocar processo em segundo plano
			  ```Bash
			  bg
			  ```
			  Desvincula o processo do terminal, garantindo que continue rodando ao fechar o terminal.
			  ```Bash
			  dissown
			  ```
			- **Rodar Logseq em `flatpak`**
			  ```Bash
			  flatpak run com.logseq.Logseq
			  ```
			  **`CTRL+Z`**
			  Colocar processo em segundo plano
			  ```Bash
			  bg
			  ```
			  Desvincula o processo do terminal, garantindo que continue rodando ao fechar o terminal.
			  ```Bash
			  dissown
			  ```
			-
	- **Alternativa 2 (GUI)**: abrir ambos pelo **[Kicker]([[Lançador de Aplicativos do KDE]])**, a versão em `Flatpak` aparece como **Atalho** e a versão em `Snap` aparece como comando a **Executar**.
	  id:: 67ddf0c0-8c49-437d-b98b-4a93157cd02e
		- ![Screenshot_20250321_201916.png](../assets/Screenshot_20250321_201916_1742599172703_0.png)
-
-