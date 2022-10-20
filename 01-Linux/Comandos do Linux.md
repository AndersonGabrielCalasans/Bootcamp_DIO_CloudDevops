# Comandos do Linux

ip a -> mostra todos os ips na máquina
para acessar a máquinna remotamente do windowns é necessário o PuttY.

clear ou Ctrl+l -> limpar terminal
$ -> indica que não é um usuário admin(root)
~ -> indica que estou na pasta do usuário
date -> data e hora atual
touch arquivo.txt -> cria um arquivo

## Navegando por diretorios

pwd -> fala exatamente onde você está
cd / -> me leva para a raiz
cd pasta -> me leva ao diretorio indicado
cd .. -> voltar a um diretório anterior
cd ../pasta -> volta um dir e já entra em pasta
ls -> lista os arq e dir no local

## Filtrar exibição de arquivos

ls | more -> lista com rolagem
Ctrl+c -> fecha a visualização
ls pa (press Tab+Tab)-> retorna todos arq que começam com 'pa' no dir
ls p* -> retorna todos arq que começam com 'p' no dir
ls p?s -> retorna tudo que começa com 'p', seguido de qualquer letra e depois 's'
ls arquivo[2-5]* -> lista todos arquivos do 2 ao 5
ls arquivo[2, 5]* -> lista os arquivos do 2 e 5
ls arquivo[^2-5]* ->lista todos arquivos menos o 2 ao 5
find -name arq* -> busca arquivo com nome que comece com 'arq'

## Diretórios

mkdir diretorio ou mkdir 'meu diretorio'-> cria diretório
rmdir -> exclui o diretório (caso esteja vazio)
rm -> exclui arquivo
rm -rf Documentos -> exclui tudo que tem dentro e também o diretório Documentos
rm -rfv Documentos -> exclui tudo que tem dentro e também o diretório Documentos e diz o que está passando

man comando -> também obtme ajuda mas dá uma descrição de cada função
comando --help -> **Ajuda**, lista os parametros
exemplo:
ls --help
ls -l -> lista longa de todos os objetos do dir

gabriel@linux:/$ ls -l
total 1903684
lrwxrwxrwx   1 root root          7 ago  9 11:53 bin -> usr/bin
drwxr-xr-x   4 root root       4096 out 13 20:48 boot
drwxr-xr-x  20 root root       4080 out 14 13:28 dev
drwxr-xr-x  97 root root       4096 out 13 20:54 etc
drwxr-xr-x   3 root root       4096 out 13 20:54 home
lrwxrwxrwx   1 root root          7 ago  9 11:53 lib -> usr/lib
lrwxrwxrwx   1 root root          9 ago  9 11:53 lib32 -> usr/lib32
lrwxrwxrwx   1 root root          9 ago  9 11:53 lib64 -> usr/lib64
lrwxrwxrwx   1 root root         10 ago  9 11:53 libx32 -> usr/libx32
drwx------   2 root root      16384 out 13 20:41 lost+found
drwxr-xr-x   2 root root       4096 ago  9 11:53 media
drwxr-xr-x   2 root root       4096 ago  9 11:53 mnt
dr-xr-xr-x 165 root root          0 out 13 20:51 proc
drwxr-xr-x  28 root root        840 out 14 13:32 run
lrwxrwxrwx   1 root root          8 ago  9 11:53 sbin -> usr/sbin
drwxr-xr-x   6 root root       4096 ago  9 11:58 snap

drwxr-xr-x -> tipo do arquivo 

se começar com:
 - dr = diretório
 - lr = link
 - - = arquivo

terminar com:
 - ------ = permissão root
 - -xr-x = permissão usuario comum

# Trabalhando com textos no linux

vi README.txt -> caso nao exista o arquivo, cria
'i' -> para entrar no menu Insert e digitar texto
'Esc' -> sair da edição
':' -> para acessar o menu do texto
'wq' -> salvar e sair
cat -> verifica o conteudo do arquivo

ou pode abrir arquivo com:
nano README.txt -> abre edição do arquivo com nano.

 
history -> mostra os últimos 1000 comandos utilizados pelo usuário
history x -> mostra os últimos x comandos utilizados pelo usuário
!x -> executa o comando x do indice do history
history | grep "comando" -> encontra todos os comandos utilizados que possuem 'comando'
export HISTTIMEFORMAT="%c " -> seta o history com data e hora padrão, pode ser alterado o formato padrão por:
%d: Day
%m: Month
%y: Year
%H: Hour
%M: Minutes
%S: Seconds
%F: Full date (Y-M-D format)
%T: Time (H:M:S format)

Dúvida: vamos aprender sobre frameworks de gestão ageis como Scrum e Kambam?