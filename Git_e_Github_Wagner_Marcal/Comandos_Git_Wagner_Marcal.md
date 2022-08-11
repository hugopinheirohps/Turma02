# Comandos

## Configuração

### Geral

As configurações do GIT são armazenadas no arquivo **.gitconfig** localizado dentro do diretório do usuário do Sistema Operacional (Ex.: Windows: C:\Users\Documents and Settings\Wagner ou *nix /home/Wagner).

As configurações realizadas através dos comandos abaixo serão incluídas no arquivo citado acima.

##### Setar usuário
	git config --global user.name "Wagner Marcal"

##### Setar email
	git config --global user.email wagner@teste.com.br

##### Listar configurações
	git config --list

### Comitar arquivo/diretório

##### Comitar um arquivo
	git commit meu_arquivo.txt

##### Comitar vários arquivos
	git commit meu_arquivo.txt meu_outro_arquivo.txt
	
##### Comitar informando mensagem
	git commit meuarquivo.txt -m "minha mensagem de commit"

### Remover arquivo/diretório

##### Remover arquivo
	git rm meu_arquivo.txt

##### Remover diretório
	git rm -r diretorio

### Visualizar histórico

##### Exibir histórico
	git log

## Repositório Remoto

### Exibir os repositórios remotos
	git remote
	git remote -v

### Vincular repositório local com um repositório remoto
	git remote add origin <url>
	
### Exibir informações dos repositórios remotos
	git remote show origin
	
### Renomear um repositório remoto 
	git remote rename origin <novoNome>
	
### Desvincular um repositório remoto
	git remote rm <repositorio>

### Enviar arquivos/diretórios para o repositório remoto
	git push origin <branch>
	git push
	

### Atualizar repositório local de acordo com o repositório remoto

##### Atualizar os arquivos no branch atual
	git pull
	
##### Buscar as alterações, mas não aplica-las no branch atual
	git fetch
	
### Clonar um repositório remoto já existente
	git clone <url>