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

* Normalmente é por meio dele que recevemos as atualizações de outros dev;
