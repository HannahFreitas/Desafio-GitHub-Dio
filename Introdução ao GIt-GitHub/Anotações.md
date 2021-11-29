# Introdução ao Funcionamento do Git

1 passo: Instalação do Git na sua máquina: 

[Git](https://git-scm.com/downloads)

## Windows 

- Aperte sobre o download
- Espera baixar
- Prossiga com Instalação
- Verifique se o git Bash foi instalado 

## Linux 

- Debian/Ubuntu:

Para o download da versão estável, abra seu terminal e digite o seguinte comando: 

A utilização do sudo é para liberar seu acesso como administrador
#$ sudo apt-get install git

## MacOS

- Precisa ter o homebrew instalado para utilização do comando disponibilizado abaixo:

#$ brew install git

## Configurando o Git Bash

- Após concluir a instalação, abra o git bash, pode-se ser acessado clicando com o lado direito do mouse na aréa de trabalho e escolher a opção "open git bash here".
- Ao abrir, insira o comando: git config --list 
=> Perceberemos que não há nada configurado, então vamos começar a configurar.

2 passo: Utilizando comandos para configurar o usuário e a senha da mesma forma que está no seu GitHub.

- Primeiro vamos configurar o usuário, utilizarei o meu usuário, troquem para o de vocês.

#$ git config --global user.name "HannahFreitas"

- Agora vamos configurar o email de usuário.

#$ git config --global user.email hannahcassia@gmail.com

- Ao digitar o comando: (git config --list) agora irá aparecer alguns dados, inclusive o que acabamos de configurar.

#$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=hannahcassia@gmail.com
user.name=HannahFreitas

- E assim, os primeiros passos para a configuração do usuário já está dada.

## Utilizando os comando no git para inserir os projetos no GitHub.

- Se for um repositório já criado, basta dar o clone com este comando e fazer suas modificações:

#$ git clone https://github.com/HannahFreitas/Desafio-GitHub-Dio.git

Isso trará tudo para dentro da sua máquina, assim podendo fazer alterações.

- Após as alterações feitas, dê o comando:

#$ git status

Assim poderemos analisar todos os arquivos que foram modificados e os que quero ou não mandar.

- Próxima etapa é adicionar os arquivos, caso queira adicionar todos os arquivos, insira o comando>

#$ git add .

- Após isso, estará pronto para dar o commit, que podemos realizar com o comando: 

#$ git commit -m "mensagem que você deseja inserir"

O -m tem o objetivo de registrar uma mensagem no seu commit.

- Este commit permite agora que você possa adicionar finalmente seus novos dados ao seu repositório, como comando:

#$ git push origin main

Main é o nome da branch original, que também pode estar declarada como master, terás de checar a branch com o comando: 

#$ git branch

E assim podendo realmente escolher a branch correta do projeto.

- Após isso, cheque se está tudo okay no seu GitHub e seja feliz.

### Caso seja a criação de um repositório para um arquivo ja existente na máquina, terá mais dois comandos:

- Para iniciar o projeto dizendo que é possível fazer o versionamento com o git:

#$ git init 

Este comando inicia o seu projeto e o deixa pronto pra versionamento.

- Agora tem que ter a ligação com o repositório criado no GitHub, usarei o meu repositório atual de exemplo.

#$ git remote add origin https://github.com/HannahFreitas/Desafio-GitHub-Dio.git

E assim, agora há a conexão linkada do git com o github. Após isso, só seguir os comandos de antes e ser feliz 🤩



