# Braches

* _Introdução da seção_

## O que é um branch?

Branch é a forma que o git **separa as versões dos projetos**;
Quando um projeto é criado ele inicia na branch **master**, estamos trabalhando nela até este ponto do curso;
Geralmente cada nova feature de um projeto **fica em um branch separado**;
Após a finaliação das alterações os **branchs são unidos** para ter o código-fonte final;

## Criando e visualizando os branches

Para visualizar os branchs disponíveis basta digitar **git branch**

Para criar um branch você precisa utilizar o comando **git branch <nome_brach>**

Estas duas operações são muito utilizadas no dia a dia de um dev;

## Deletando Branches

Podemos deletar um branch com a flag **-d ou --delete**
**Não é comun deletar um branch**,normalmente guardamos o histórico do trabalho;
Geralmente se usa o delete quando o branch foi criado errado;
comando ->
**git branch -d <nome_branch>**

## Mudando de Branch

Podemos mudar para outro branch utilizando o comando **git checkout -b <nome_branch>**
Este comando também é utilizado para dispensar mudanças de um arquivo;
Alterando o branch podemos lear alterações que foram commitadas juntos, **tome cuidado!!**

```comandos
git checkout -b nome_branch 
ele muda e criar
```

## Unindo branches

* O código de dois branches distintos pode ser unido pelo comando **git merge <nome_branch>**

* Outro comando para a lista dos **mais utilizados**;

* Normalmente é por meio dele que recebemos as atualizações de outros 
dev;

```git
git checkout main

git merge development
```

## Stash

* Podemos salvar as modificações atuais **para prosseguir com uma outra abordagem de solução** e não perder o código

* O comando para esta ação é o **git stash**

* Após o comando o branch será resetado para a sua versão de acordo com o repo;

## Recuperando stash

* Podemos verificar as stashs criadas pelo comando **git stash list**

* E também podemos recuperar a stash com o comando **git stash <nome_stash>**

* Desta maneira podemos continuar de onde paramos com os arquivos adicionados a stash

* **git stash você apaga, git stash list ver as stash salva e git stash amply id da stash recebe as stash salva**

* o comando **git stash show -p e o id** , verifica as alteração de cada uma

## Removendo a stash

* Para limpar totalmente as stash de um branch podemos utilizar o comando **git stash clear**

* Caso seja necessário deletar uma stash específica podemos utilizar **git stash drop <nome_stash>**

## Utilizando tags

* Podemos criar tags nos branches por meio do comando **git tag -a <nome_tag> -m "msg"**

* A tag é diferente do stash, serve como um **checkpoint de um branch**;

* É utilizada para demarcar estágios do desenvolvimento de algum recurso;

## Verificando e alterando tags

* Podemos verificar uma tag com o comando **git show <nome_tag>**

* Podemos trocar de tags com o comando **git checkout <nome_tag>**

* Desta maneira podemos retroceder ou avançar em checkpoints de um branch;

## Enviando e compartilhando tags

* As tags podem ser **enviadas para o repositório de código**, sendo compartilhada entre dos devs;

* O comando é **git push origin <nome>**

* Ou se você quiser enviar mais tags **git push origin --tags**
