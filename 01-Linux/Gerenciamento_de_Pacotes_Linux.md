## Gerenciamento de Pacotes Linux

Comando geral para gerenciar pacotes:
		apt-get 
		apt-get --help

Mostra os packs instalados
		apt list --installed

Mostra os packs que podem ser atualizados
		apt list --upgradeable

Localiza o apt pelo nome
		apt search samba

Instala um apt
		apt install <NOME DO APT>

Para realizar um download de arquivo
		wget <link formato http> 

Descompactar arquivo
		apt install unzip
		unzip arquivo.zip

Para desinstalar um apt, ex(unzip)
		apt remove unzip
Se eu adcionar o -y ao final do comando, ele pula a confirmação.

Link de todos os apt oficiais do ubuntu
		apt edit-sources

Caso eu precise add um reposítório novo é só adcionar no edit-sources.

## Atualização de SO

O ideal é que antes de realizar uma atualização você crie uma cópia de segurança de antes da atualização e depois atualize e para atualizar:

		apt update
		apt upgrade

Caso tenha algum problema no funncionamento da aplicação, é só voltar a versão antes da atualização e continuar a utilizá-la normalmente.

**Observação**: Caso não esteja no usuário root, utilizar o **sudo**, antes dos comandos.

No Ubuntu e Debian os arquivos execultaveis são .deb
No Fedora e openSUSE são .rpm

# Gerenciamento de discos Linux

Entra no diretorio do disco 2:
		fdisk /dev/sdb

Dentro do disco, aperta m para saber as opções disponiveis, n para adcionar uma nova partição.
p -> partição primária
e -> partição extendida
Particion number (default 1)
enter
enter
w -> para salvar operação e sair

**Formatando o novo disco**
		mkfs.ext4 /dev/sdb
		-y para confirmar

