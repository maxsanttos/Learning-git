# Compartilhamento e atualização

## Encontrando branches

* Branches novos são criados a todo tempo e o **seu git pode não estar mapeando eles**;

* Com o comando **git fetch** você é atualizado de todos os branchs e tags que ainda não estão reconhecidos por você;

* Este comando é útil para utilizar o branch de algum outro dev do time, por exemplo;

## Recebendo alterações

* O comando **git pull** serve para recebermos atualizações do repositório remoto;

* Cada branch pode ser atualizado coom o git pull;

* Utilizamos para atualizar a master do repo como também quando trabalhamos em conjunto e queremos receber as atualizações de um dev;

## Enviando alterações

* O comando **git push** faz o inverso do pull, ele envia as alterações para o repo remoto;

* Serve também para **enviar as atualizações de um branch específico** para outro dev;

* Ou quando terminamos uma tarefa e precisamos enviar ao repo;

## Utilizando o remote

* Com o **git remote** podemos fazer algumas ações como: adicionar um repo trackear ou remover;

* Quando criamos um repo remoto, adicionamos ele ao git com **git remote add origin link**

```gitexemple
git remote add origin https://git.com/maxsanttos...
```

## Trabalhando com submódulos

* Submódulos é a maneira que temos de possuir **dois ou mais projetos em um só repositório**;

* Podemos adicionar uma dependência ao nosso projeto atual, porém mantendo suas estruturas separadas;

* Para adicionar o submódulos utilizamos o comando **git submodule add <link_repo>**

* Para verificar os submódulos o comando é **git submodule**

## Atualizando submódulo

* Para atualizar um submódulo primeiro devemos **commitar as mudanças**;

* E para enviar para o repo do submódulo utilizamos **git push --recurse-submodules=on-demand**

* Este fluxo fará a atualização apenas do submódulo;
