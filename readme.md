# One Page com parallax

Projeto desenvolvido para estudo com aplica��o das seguintes features:

- HTML
- CSS

## Screenshot

![](../assets/images/screenshot-desktop.png)

### O que aprendi

No decorrer da cria��o deste projeto eu aprendi novas formas de utilizar classes, pseudo-classes e propriedades de CSS:

- :target

> Utilizado para fazer modifica��es no 'alvo', como aplicar bordas, background margem, etc... Ex:

`/* Seleciona um elemento com a ID correspondente ao fragmento da URL */
:target {
  border: 2px solid black;
}`

- scroll-behavior: smooth;

> Aplica um comportamento suave ao scroll quando se utiliza �ncoras (#) nos links, ex.:

`html {
    scroll-behavior: smooth;
}`

- scroll-margin-top: value

> Adiciona espa�amento entre o elemento alvo da �ncora (#) e o topo da viewport, ex.:

`article:target {
    scroll-margin-top: 10vh;
}`

- menu mobile com cess puro

> Inseri um simples input:checkbox no header com uma label, nela coloquei o atributo for com o mesmo dado do id do input
> No CSS ocultei esses elementos, e nas resolu��es mobile apliquei display flex para exibir as linhas da label, formatei os itens do menu da forma como desejei exibir nas dimens�es mobile e apliquei o display: none, feito isso apliquei no seletor do input:checkbox para que quando a pseudo-clase :checked for selecionada, seria aplicado no menu o display: block

`header input[type=checkbox]:checked ~ nav {
    display: block;
}
header input[type=checkbox]:checked ~ label {
    height: 30px;
}`