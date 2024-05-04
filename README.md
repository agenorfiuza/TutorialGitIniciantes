<h1 style="color : blue">
    TUTORIAL GIT/GITHUB DOS COMANDOS BÁSICOS PARA INICIANTES.
</h1>

<p style="color : white; font-size : 18px;">
    Tutorial dos comandos básicos do Git e interação com o GitHub.
</p>

<h2 style="color : #2188db">
    MAS ANTES VEREMOS ALGUNS COMANDOS DE TERMINAL:
</h2>

<p style="color : white; font-size : 18px;">
    CLEAR - limpa a tela do terminal:
</p>

```
$ clear
```

<p style="color : white; font-size : 18px;">
    LS - lista arquivos e pastas do diretório:
</p>

```
$ ls
$ ls -a "exibe arquivos ocultos"
```

<p style="color : white; font-size : 18px;">
    CD - abre uma pasta:
</p>

```
$ cd pasta
$ cd pasta\outro
```

<p style="color : white; font-size : 18px;">
    CD .. - retorna para a pasta anterior:
</p>

```
$ cd ..
$ cd ../outra-pasta "sai do diretório atual e já abre outro dentro do mesmo diretório"
```

<p style="color : white; font-size : 18px;">
    TOUCH - cria arquivos:
</p>

```
$ touch aula-de-git.txt
$ touch arquivo\outro\aula-de-git.txt
```

<p style="color : white; font-size : 18px;">
    RM - deleta um arquivo:
</p>

```
$ rm aula-de-git.txt
```

<p style="color : white; font-size : 18px;">
    MKDIR - cria uma pasta:
</p>

```
$ mkdir pasta
$ mkdir pasta\outro
```

<p style="color : white; font-size : 18px;">
    MV - renomeia o nome da pasta:
</p>

```
$ mv pasta pasta1proj
```

<p style="color : white; font-size : 18px;">
    RMDIR - deleta uma pasta:
</p>

```
$ rmdir pasta
$ rmdir pasta\outro
```

<p style="color : white; font-size : 18px;">
    NANO - editor de texto para terminal:
</p>

```
$ nano arquivo.txt
```

<p style="color : white; font-size : 18px;">
    CAT - exibe o conteúdo do arquivo no terminal:
</p>

```
$ cat arquivo.txt
```



























<h2 style="color : #2188db">
    COMO SABER A VERSÃO INSTALADA DO GIT?
</h2>

<p style="color : white; font-size : 18px;">
    Para saber a versão instalada não tem mistério, basta digitar a seguinte linha de comando:
</p>

```
$ git --version
```

<h2 style="color : #2188db">
    COMO VERIFICAR A ATUAL LISTA DE CONFIGURAÇÕES GLOBAIS DO GIT?
</h2>

<p style="color : white; font-size : 18px;">
    Para verificar as configurações do Git, basta digitar a seguinte linha de comando:
</p>

```
$ git config --global --list
```

<p style="color : white; font-size : 18px;">
    Para sair da lista, digite a letra Q.
</p>

<h2 style="color : #2188db">
    COMO INSERIR O NOME E O EMAIL GLOBAL?
</h2>

<p style="color : white; font-size : 18px;">
    Para isso, basta digitar as seguintes linhas de comando:
</p>

```
$ git config --global user.name "Agenor Fiuza"
$ git config --global user.email afiuzane@gmail.com
```

<h2 style="color : #2188db">
    COMO CRIAR UM REPOSITÓRIO LOCAL PELO TERMINAL?
</h2>

<p style="color : white; font-size : 18px;">
    1 - crie a pasta do repositório
</p>
<p style="color : white; font-size : 18px;">
    2 - abra a pasta do repositório
</p>
<p style="color : white; font-size : 18px;">
    3 - inicialize o repositório
</p>

```
$ mkdir projeto1
$ cd projeto1
$ git init
```

<h2 style="color : #2188db">
    COMO VISUALIZAR ARQUIVOS E PASTAS OCULTAS PELO TERMINAL?
</h2>

<p style="color : white; font-size : 18px;">
    Após criar o repositório e inicializar, o git irá criar uma pasta oculta para salvar as configurações. O nome desta pasta é (.git).
</p>
<p style="color : white; font-size : 18px;">
    Para visualizar e abrir a pasta  faça o seguinte: "ls -a" vai exibir a pasta oculta e "cd .git" vai abrir a pasta. Logo em seguida "ls" vai listar os arquivos e pastas dentro dela.
</p>

```
$ ls -a
$ cd .git
$ ls
```

<h2 style="color : #2188db">
    COMO VERIFICAR O STATUS ATUAL DO REPOSITÓRIO LOCAL?
</h2>

<p style="color : white; font-size : 18px;">
    O comando para verificar o status atual do repositório local vai retornar 3 tipos de informação:
</p>

<p style="color : white; font-size : 18px;">
    1 - Retorna a branch atual
</p>
<p style="color : white; font-size : 18px;">
    2 - Retorna se existe algum arquivo commitado
</p>
<p style="color : white; font-size : 18px;">
    3 - e se existe algum arquivo untracked para ser adicionado/rastreado para ser commitado
</p>

```
$ git status
```

<h2 style="color : #2188db">
    COMO ADICIONAR UM ARQUIVO NÃO RASTREADO PARA SER COMMITADO, OU SEJA, PARA O STAGE?
</h2>

<p style="color : white; font-size : 18px;">
    O comando para adicionar um arquivo não rastreado para ser commitado:
</p>

```
$ git add arquivo.txt
$ git add . 

<para adicionar vários arquivos de uma só vez>
```

<h2 style="color : #2188db">
    COMO RETORNAR UM ARQUIVO PARA O UNSTAGE?
</h2>

<p style="color : white; font-size : 18px;">
    Caso haja arrependimento e queira retornar ao estágio anterior digite o seguinte comando:
</p>

```
$ git rm --cached arquivo.txt
```

<h2 style="color : #2188db">
    COMO COMMITAR UM ARQUIVO?
</h2>

<p style="color : white; font-size : 18px;">
    Após a modificação no repositório e adicionar as atualizações no stage, devemos commitar as alterações :
</p>

```
$ git commit -m "arquivo.txt modificado no paragrafo final"
```

<h2 style="color : #2188db">
    COMO VER O COMMIT REALIZADO?
</h2>

<p style="color : white; font-size : 18px;">
    O LOG de commits exibe o nome da branch, o autor do commit, a data/hora e msg. Para ver um histórico de commits realizado, basta digitar a seguinte linha de comando:
</p>

```
$ git log 

<para sair da tela de log, basta digitar a letra q>

$ git log --oneline 

<forma enxuta de exibição em uma linha>
```

<h2 style="color : #2188db">
    COMO REVERTER O COMMIT REALIZADO?
</h2>

<p style="color : white; font-size : 18px;">
    Existe 3 formas de reverter um commit:
</p>

<p style="color : white; font-size : 18px;">
    1 - CHECKOUT: retorna para um ponto anterior do seu projeto sem alterar sua linha do tempo. Vc pode simplismente olhar ou criar uma nova branch a partir daquele ponto e depois retorna para o último estágio.
</p>

```
$ git log --oneline 

<copia a id do commit>

$ git checkout b804c3d 

<então retorna para este commit na linha do tempo>

$ git checkout main 

<retorna para o último estágio que estava>
```

<p style="color : white; font-size : 18px;">
    2 - REVERT: retorna para um ponto anterior do seu projeto para que seja o ponto atual, mas também mantem a linha do tempo do projeto, em caso de arrependimento. Deve ser feita com consciencia.
</p>

```
$ git log --oneline
$ git revert b804c3d 

<na tela que abrir digite :q>

$ git log --oneline
```

<p style="color : white; font-size : 18px;">
    3 - RESET: retorna para um ponto anterior do seu projeto e deleta todos os commits superiores. Máxima atenção nesta etapa.
</p>

```
$ git log --oneline
$ git reset b804c3d --hard
$ git log --oneline 

<vai exibir o histórico até o commit selecionado e apagar as outras mais novas>
```

<h2 style="color : #2188db">
    COMO JUNTAR VÁRIOS COMANDOS DO GIT EM UMA SÓ LINHA?
</h2>

<p style="color : white; font-size : 18px;">
    Para isso deve-se utilizar (&&) entre os comandos:
</p>

```
$ git add . && git commit -m "arquivo.txt modificado no paragrafo final"
```

<h2 style="color : #2188db">
    COMO FAZER O GIT IGNORAR OU NÃO RASTREAR UM ARQUIVO OU PASTA?
</h2>

<p style="color : white; font-size : 18px;">
    Para isso deve-se criar um arquivo chamado .gitignore e colocar o nome dos arquivos e/ou pastas nele:
</p>

```
$ touch .gitignore 

<digite o nome do arquivo ou pasta. Ao utilizar o git add o arquivo ou pasta não irão ser visiveis ao git>

$ git add .
$ git commit -m "adicionado o .gitignore"
```

<h2 style="color : #2188db">
    COMO SABER A BRANCH OU LISTA DE BRANCH DO REPOSITÓRIO ATUAL?
</h2>

<p style="color : white; font-size : 18px;">
    Este comando vai listar as branchs do repositório atual:
</p>

```
$ git branch 
```

<h2 style="color : #2188db">
    COMO CRIAR UMA BRANCH?
</h2>

<p style="color : white; font-size : 18px;">
    Para criar uma nova branch a partir da atual (a branch atual pode ser vista listando as branch como visto na linha de comando anterior, sendo que a atual será exibida com um asterisco), basta digitar a linha de comando e o nome da nova branch:
</p>

```
$ git branch teste
```

<h2 style="color : #2188db">
    COMO MUDAR DE BRANCH?
</h2>

<p style="color : white; font-size : 18px;">
    Para transitar entre as branchs, basta digitar a seguinte linha de comando e o nome da branch:
</p>

```
$ git checkout teste
```

<h2 style="color : #2188db">
    COMO DELETAR UMA BRANCH?
</h2>

<p style="color : white; font-size : 18px;">
    Para deletar uma branch, basta digitar a seguinte linha de comando com o -d e o nome da branch.:
</p>

```
$ git branch -d teste 

<caso haja atualizações para fundir a branch ao original, o sistema não permitirá a exclusão. Mas caso vc queira excluir mesmo com as atualizações, basta digitar -D maiúsculo>

$ git branch -D teste
```

