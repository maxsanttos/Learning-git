# Análises e inspeção

## Exibindo informações

* O comando **git show** nos dá diversas informações úteis;

* Ele nos dá as informações do branch atual e também **seus commits**;

* As **modificações de arquivos** entre cada commit também são exibidas;

* Podemos exibir as informações de tags também com: **git show <nome_tag>**

## Exibindo diferenças

* O comando **git diff** serve para exibir as diferenças de um branch;

* Quando utilizado as diferenças do branch atual com o remoto serão exibidas no terminal;

* Podemos também verificar a diferença entre arquivos:**git diff <arquivo_a> <arquivo_b>**

## Log resumido

* O comando **git shortlog** nos dá um log resumido do projeto;

* Cada commit será unido por **nome do autor**;

* Podemos então saber quais commits foram enviados ao projeto e por quem;

## Utilizando o describe

* Com o comando **git describe --tags** podemos verificar todas as tags do nosso projeto;

* Com a opção --all recebems também a referência das tags;
