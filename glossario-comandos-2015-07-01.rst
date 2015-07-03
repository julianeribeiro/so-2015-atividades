======================
Glossário de comandos
======================

:Disciplina: Fundamentos de Sistemas Operacionais
:Professor: Jurandy Soares
:Nome: Juliane Paula Vieira Ribeiro
:Matrícula: 20121144010036
:Data: 01.07.15

cat
"Change archive text". Através dele posso entrar em arquivos de texto e ver o seu conteúdo;
Ex: cat NOMEDOARQUIVO.txt

cd
"Change directory" . Possibilita a navegação por diretórios (pastas), ou seja, através dele posso entrar e sair de diretórios.
Ex: cd /home/$USER
(Vai para o diretório do usuário).

cowsay
Forma de imprimir mensagens no terminal e enviar mensagens pela rede;
Ex: cowsay  "Hello world".
      
echo
Exibe uma mensagem em meu shell. Escreve num arquivo de texto.
Ex: echo TEXTO >> NOMEDOARQUIVO.txt
Ex: echo  $HOME.
        
env
Executa um programa em um ambiente modificado. Porém, sem qualquer argumento lista as variáveis de ambiente que estão definidas.
Ex: env –i: Ignora todas as variáveis de ambiente e inicializa um ambiente vazio.
obs: Variaveis de ambiente são espaços de memória que armazenam valores, que nada mais são do que definições e valores que, tanto o shell como outros programas utilizam para configuração do ambiente do usuário no momento em que é realizado o login, sendo algumas: HOME, SHELL, TERM, USER, etc.
exit
Finaliza um login no terminal, ou seja, faz logout da sessão atual.
Ex: exit.
        
help
Exibe informações sobre os comandos internos. Ou seja, sempre que se existir dúvidas e se quiser saber mais sobre o comando em questão basta usá-lo.
Ex: help logout.

HISTTIMEFORMAT 
Possibilita personalizção das informações do histórico, mostra-se, portanto, a data e a hora que os comandos foram executados.
Ex: HISTTIMEFORMAT="%d/%m/%y%T". No caso, mostra-se o dia, mês, ano e hora da execução dos comandos.
 
hostname        
Informa o nome da máquina.
Ex: hostname

ifconfig
Permite configurar as interfaces da rede, ou seja, é utilizado na inicialização do sistema para configuração destas interfaces.	Este é um comando de argumento, porém pode ser apresentado com comando ou não, caso não seja passado junto ao comando o mesmo era apenas exibir o estado das interfaces atualmente definidas.
Ex: ifconfig eth0. Exibirá o estado e informações da interface de rede eth0
        
last
Mostra informações sobre últimos logins, ou seja, exibe informações quanto a entrada e saída de usuários do sistema. Pode ser usado seguido de um argumento 
Ex: last -10. Nessa caso, será mostrado informações sobre os dez últimos logins.
Ex: last reboot: Mostra as reinicializações do sistema.
Ex: last juliane: Mostra somente atividades do usuário juliane.

lastb
Possibilita que o usuário verifique se houveram tentativas mal sucedidas de ingresso no sistema.
Ex: lastb $USER;

ls  
Lista diretórios e tudo aquilo que disponível para o usuário. Através desse comando é possível ver os arquivos existentes dentro de uma pasta (diretório).
Ex: cd /home/juliane > ls

mkdir
"Make diretório". Cria um novo diretório.
Ex: mkdir $USER;
   
nome="fulano"
Declaração de uma variável. As variáveis do sistema servem para armazenar algum valor. Uma declaração é feita da seguinte maneira: NOME="VALOR";
Ex: var="Juliane"

passwd
Possibilita que um usuário logado altera sua senha ou que o administrador altere a senha de algum usuário. Seguido de argumento possibilita algumas coisas ao administrador, como por exemplo "sudo passwd -l fulano", bloqueando a conta do usuário "fulano".
        
pwd
Mostra em que lugar o usuário está, ou seja, mostra o diretório corrente.  Extremamente para situar o usuário e saber em que diretório ele se encontra.
Ex: pwd.

set
Lista todas as variáveis de ambiente do usuário tais como o nome da máquina, arquitetura da máquina, usuário logado, etc. É possível ativar as várias opções paraset com um - e desativá-las com um +.

tree
Serve para listar o conteúdo de um diretório em formato de árvore. A única maneira do comando ls está na forma como as informações são exibidas.
Ex: tree –f.

tty
"Teletype".É simplismente o terminal ao qual se está conectado.
Ex: tty –help.

vim
É um editor de textos, podendo ser de três formas: modo de linha, modo de edição e modo de comandos

wait
Espera que um comando seja concluído e retorna seu estado de saída.
Ex: wait 2017.

wall
Envia mensagens para os terminais dos usuários em rede. A mensagem deve ser escrita e ao final se pressionar ctrl+d para enviar a mensagem.
Ex: wall 'Olá, pessoas'.

which
Usado para fazer buscas rápidas de arquivos no sistema, ou seja, através dele pode-se encontrar o caminho onde se encontram determinados comandos.
Ex: which java
  
while
Tanto while, until e for são comandos para repetição de código. Ou seja, executa um bloco de comandos enquanto uma condição for verdadeira.
Ex: while [ 1 ] ; do clear; w ; sleep 2; done.
       
who
Mostra quem está conectado ao sistema nesse momento ;
Ex: who

whoami
"Quem sou eu". Mostra quem é o usuário que primeiro logou, que está logado no sistema;
Ex: whoami
    
write
Escreve mensagens para outro usuário em rede.

OUTROS
bin
Contém arquivos programas que são usados com frequência pelos usuários. Armazena os executáveis de alguns comandos básicos do sistema, como o sur, tar, cat, rm, pwd, etc.
/var
Dados variáveis, como arquivos e diretórios de spool, dados de administração e login, e arquivos transitórios.

cd..
Sai do seu atual diretório, indo para um diretório acima.
cd ~
Volta para o seu diretório (/home).
cd –
Volta para o diretório anterior.
mv
"Move". Com ele posso renomear de um diretório e também movê-lo;
Ex: mv NOMEANTIGO NOVONOME (Renomeação)
Ex2: mv NOMEDODIRETÓRIO NOVOENDEREÇOPARAONDEVOUMANDAR.
rmdir
"Remove directory". Remove diretórios.
Ex: rmdir NOME DA PASTA.

