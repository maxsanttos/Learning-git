# Curso_git

Aprendendo git

## Comandos fundamentais

* _Introdução da seção_

## O que é um repositório?

É onde o código será **armazenado**;
Na maioria das vezes cada projeto tem **um repositório**;
Quando criamos um repositório estamos iniciando um projeto;
O repositório pode ir para servidores que são especializados em gerenciar repos, como:**GitHub** e **Bitbucket**;
Cada um dos desenvolvedores do time pode baixar o repositório e **criar versões diferentes** em sua máquina;

## Criando repositórios

Para criar um repositório utilizamos o comando:**git init**
Desta maneira o git vai criar os arquivos necessários para iniciallizá-lo;
Que estão na pasta oculta **.git**;
Após este comando o diretório atual **será reconhecido pelo git como um projeto** e responderá aos seus demais comandos;

## O que é o GitHub?

É um **serviço para gerenciar repositórios**, gratuito e amplamente utilizado;
Podemos **enviar nossos projetos** para o GitHub e disponibilizá-lo para outros devs;
O GitHUb é gratuito tanto para projetos públicos como **privados**;
Vamos criar uma conta em:<https://github.com>

## Mudança do nome principal de branch

Olá pessoal!

Há um tempo atrás houve uma mudança no GitHub, o branch principal se chamava master e agora se chama main, então pode ser que haja essa diferença de nomenclatura ao longo do curso, você só precisa trocar onde estiver master para main.

Na prática não muda em nada, é apenas uma alteração de nomenclatura, inclusive podemos criar o nosso repositório com o nome de master como o branch principal, isso é configurável e permitido. O que acontece é que a sugestão feita pelo GitHub como branch principal agora tem o nome de main.

Um abraço a todos!

## Enviando repositório para o GH

Podemos facilmente **enviar nossos repos** para o GitHUb;
Precisamos criar o projeto no GitHub, inicializar o mesmo no git em nossa máquina, sincronizar com GH e enviar;
E esta sequência que parece ser complexa é facilmente executada **por poucos comandos**;
Vale lembrar que só fazemos **uma vez por projeto** este fluxo;
Porém alguns dos comandos utilizados vão ser úteis ao longo do curso;

## Comandos do git

## ...Or create a new repository on the command line

echo "# curso_git" >> README.md

git init

 1º git add README.md

2º git commit -m "first commit"

3º git push -u origin master

git branch -M master - para criar uma branch

## Adcionando uma origem

tem duas formas ->

git remote add origin <git@github.com:maxsanttos/Curso_git>

git  remote add origin <https://github.com/maxsanttos/Curso_git>

## Remover a origem atual

git remote -v - ver as origins

git remote rm origin - para remover

## Verificando mundanças do projeto

As mundaças do projetos podem ser verificadas por:**git status**
Este comadno é utilizado **muito frequentemente**;
Aqui serão mapeadas todas as alterações do projetos;
Como:**arquivos não monitorados** e **arquivos modificados**;
Podemos também dizer que é a **diferença** do que já está enviado ao servidor ou salvo no projeto;

## Adicionando arquivo ao projeto

Para adcionar arquivos novos a um projeto utilizamos:**git add**
Podemos adcionar **um arquivo** específico como também **diversos de uma vez só**;

Somente adicionando arquivos eles serão monitorados pelo git;
Ou seja, **se não adicionar ele não estará** no controle de versão;
É interessante utilizar este comando de tempos em tempos para não perder algo por descuido;

COMANDOS

Para adicionar tudo

git add .  -> ele adciona todos os arquivos criatos para serem committed

## Salvando alterações do projeto

A alterações salvas do projetos são realizadas por:**git commit**
Podemos commitar **arquivos específicos** ou vários de uma vez com a flag **-a**
É uma boa prática enviar **uma mensagem a cada commit**, com as alterações que foram feitas;
A mensagem podem ser adicionada com a flag **-m**

### Comando para enviar todos ou commitar todos

git commit -a -m "uma_mensagem"

## Enviando código ao repo remoto

Quando finalizamos uma funcionalidade nova,**enviamos o código ao repositório remoto**, que é código-fonte;

Esta ação é feita pelo **git push**
Após esta ação **o código do servidor será atualizado baseando-se no código local** enviado;

## Recendo as mundanças

É comun também ter que **sicronizar o local** com as mudanças do remoto;
Esta ação é feita pelo **git pull**

Após o comando serão **buscadas atualizações**, se encontradas elas **serão unidas ao código atual** existente na nossa máquina;

## Clonando repositórios

O ato de baixar um repositório de um servidor remoto é chamado de **clonar repositório**;
Para esta ação utilizamos o **git clone**
Passando a **referência** do repositório remoto;
Este comando é utilizado quando **entramos em um novo projeto**,por exemplo;

### Comando

git clone <https://github.com/maxsanttos/Curso_git.git>

## Removendo arquivos do repo

Os arquivos **podem ser deletados da monitoração** do git
O comando para deletar é **git rm**
Após deletar um arquivo do git ele não terá mais suas atualizações consideradas pelo git;
Apenas quando for adicionando novamente pelo **git add**

COMANDO
**git rm about.html**

## Histórico de alterações

Podemos **acessar um log** de modificações feitas no projetos;
O comando para este recurso é **git log**
Você receberá uma informação dos **commits realizados** no projeto até então;
Para sair é só aperta a tecla **q ou ctrl+c**

## Renomeando arquivos

Com o comando **git mv** podemos renomear um arquivo;
O mesmo também pode ser **movido para outra pasta**;
E isso fará com que este novo arquivo **seja monitorado pelo git**;
O arquivo anterior é **excluído**;

## Desfazendo alterações

O arquivo modificado pode ser **retornado ao estado original**;
O comando utilizado é o **git checkout**
Após a utilização do mesmo o arquivo sai do staging;
Caso seja feita uma próxima alteração, ele entra em staging novamente;
**git checkout <nome_arquivo>**

## Ignorando arquivos no projetos

Uma técnica muito utilizada é **ignorar arquivos do projeto**;
Devemos inserir um arquivo chamado **.gitignore** na raiz do projeto;
Nele podemos inserir os arquivos que não devem entrar no versionamento;
Isso é útil para **arquivos geredos automaticamente** ou arquivos que contém **informações sensíveis**;

## Desfazendo todas as alterações

Com o comando **git reset** podemos resetar as mundaças feitas
Geralmente é utilizado com a flag **--hard**

Todas as alterações **commitadas** e **também as pendentes** serão excluídas;

comando ->
**git reset --hard origin/master**

## Braches

* _Introdução da seção_

## O que é um branch?

Branch é a forma que o git **separa as versões dos projetos**;
Quando um projeto é criado ele inicia na branch **master**, estamos trabalhando nela até este ponto do curso;
Geralmente cada nova feature de um projeto **fica em um branch separado**;
Após a finaliação das alterações os **branchs são unidos** para ter o código-fonte final;

## Criando e visualizando os branches

Para visualizar os branchs disponíveis basta digitar **git branch**

Para criar um branch você precisa utilizar o comando **git branch <nome_brach >**

Estas duas operações são muito utilizadas no dia a dia de um dev;

## 