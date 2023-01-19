# GITHUB PAGES

## O que é GitHub Pages

* Uma forma de criar uma página estáticas nos **servidores do GitHub**;

* Ou seja, uma alternativa **gratuita** para hospedar nosso porfólio;

* Muito simples de colocar no ar, **não precisa de domínio ou servidor**;

* Muitas empresas utilizam para **apresentar o seu projeto** ou **a própria documentação**;

## Como criar a página

* Você deve seguir alguns passos simples, veja:

1. Criar um repositório com o nome **nomedousuario.github.io**

2. Clonar o repositório no nosso computador

3. Adicionar o código do projeto na **Branch Master**

4. Enviar o código por meio de **push**

5. E pronto, você tem um site em **<https://nomedousuario.github.io>**

## A importância do commit

* **O problema:** commits sem sentido atrapalham o projeto;

* Precisamos padronizar os commits, para que o projeto cresça de forma saudável também no versionamento, isso ajuda em:

* Review do **Pull Request**;

* Melhoraia dos log em **git log**;

* Manutenção do projeto(voltar código, por exemplo);

## Branches com commits ruis

* Há uma solução chamada **private branches**;

* Onde criamos branches que **não serão compartilhados no repositório**, então podemos colocar qualquer commit;

* Ao fim da solução do problema podemos fazer um **rebase**;

* O comando será: git rebase <nome_atual> <nome_funcionalidade> -i

* Escolhemos os braches para excluir (**squash**) e renomear com (**reword**)

## Boas mensagens de commit

* Separar **assunto** do corpo da mensagem;

* Asssunto com **máximo 50 caracteres**;

* Assunnto com **letra inicial maiúscula**;

* Corpo com no **máximo 72 caracteres**;

* Explicar o **porque e como** do commit, e não como o código foi escrito;

Fim!
