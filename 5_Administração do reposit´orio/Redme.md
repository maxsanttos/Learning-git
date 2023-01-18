# Administração do repositório

## Limpando arquivos untracked

* O comando **git clean** vai verificar e limpar arquivos não estão sendo trackeados;

* Ou seja, todos que você **não utilizou git add;**

* Utilizado para arquivos que são **geredos automaticamente**, po exemplo, e atrapalham a visualização do que é realmente importante;

## Otimizando o repositório

* O comando **git gc** é uma abreviação para **garbage collector**;

* Ele identifica arquivos que **não são mais necessários** e os exclui;

* Isso fará com que o repositório seja otimizado em questão de **performance**;

## Chegando integridade de arquivos

* O comando **git fsck** é uma abreviação de File System Check;

* Esta instrução verifica a integridade de arquivos e sua conectividade;

* Verificando assim possível **corrupções em arquivos**;

* **Comando de rotina**, utilizado para ver se está tudo ceerto com nossos arquivos;

## Reflog

* O **git reflog** vai mapear todos os seus passos no repositório, até uma mudança de branch é inserida neste log;

* Já o **git log**, que vimos anteriormente, apenas armazena os commits de um branch;

* Os **reflogs ficam salvos até expirar**, o tempo de expiração padrão é de 30 dias;

## Recuperando arquivos com reflog

* Podemos avançar e também retroceder nas **hashs** do reflog;

* Para isso utilizamos o comando **git reset --hard <nome_hash>**

* Caso você tenha algo que queira salvar, pode utilizar o **git stash** antes;

* **Lembrando:** o reflog expira com o tempo!

## Transformando o repo para arquivo

* Com o comando git archive podemos transformar o repo um arquivo compactado, por exemplo;

* O comando é **git archive --format zip --output master_files.zip master** obs:agora é main

* E emtão a master vai estar zipada no arquivo master_files.zip
