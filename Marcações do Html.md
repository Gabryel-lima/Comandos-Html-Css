## `<!DOCTYPE html>`

Informa ao navegador que esse documento é do tipo HTML e sua versão. Quando está escrito apenas html, indica que é a mais recente...

## `<html>`

Representa a raiz do documento, serve com um container que engloba todos os outros elementos HTML.

## `<body>`

É onde fica todo o conteúdo de texto, imagem e vídeos, em que o usuário vê e interage, nele os conteúdos são estruturados pelas demais tags do HTML.

## `<script>`

Esse elemento contém instruções de script ou aponta para um arquivo de script externo por meio do atributo src.

## `<head>`

Compreende as informações do documento que serão interpretadas pelo navegador (metadados). Como por exemplo, título do documento, links para folhas de estilo etc.

## `<meta>`

Define metadados, ou seja, informações sobre dados de um documento HTML. As `<meta>` tags vão dentro do elemento `<head>` e são usadas para especificar o conjunto de caracteres, o autor do documento, as configurações da janela de visualização etc.

## `<link>`

É uma tag vazia, que contém apenas atributos e faz a relação do documento HTML com recursos externos, é comumente usado para vincular uma folha de estilo externa, também é usada para definir o favicon da página (ícone da aba do navegador), como outros recursos.

## `<style>`

Essa tag é usada para declarar estilos (CSS) para um documento.

### Tags semânticas

Tags semânticas são tags que possuem um significado, que dão sentido a informação de texto ao navegador e buscadores, como por exemplo, utilizar a tag `<header>` para cabeçalhos ou `<article>` para dar um significado de artigo para aquele bloco de texto, até mesmo `<p>` para indicar que aquele texto é um parágrafo, é uma boa prática tentar sempre utilizar essas tags semânticas para ajudar no entendimento do código, além de ajudar muito no [SEO](https://www.alura.com.br/artigos/seo-o-que-e-boas-praticas-ferramentas-estrategia) do site (Otimização para motores de busca, é o que ajuda o seu site a se rankear melhor nos motores de buscas como o Google). Segue abaixo a lista de tags semânticas citadas durante o artigo:

* `<header>`
* `<main>`
* `<footer>`
* `<section>`
* `<article>`
* `<aside>`
* `<nav>`
* `<ol>`
* `<ul>`
* `<li>`

Exemplo de estruturação com tags semânticas:

![A imagem mostra os principais elementos container semânticos presentes dentro de uma página web. Elemento nav está no topo da página ocupando a largura de 100% da página. Abaixo do nav e à esquerda, há o elemento header e abaixo dele, há dois elemento sections que juntos ocupam toda a largura do header. Abaixo do nav e à direita, há o elemento aside, mais estreito e com uma extensão de altura que vai do início do header até o final dos sections. Após todos esses elementos, encontra-se o footer, que assim como o nav, ocupa 100% da largura da página.](https://www.alura.com.br/artigos/assets/o-que-e-html-suas-tags-parte-1-estrutura-basica/imagem2.jpg)

### Tags sem semântica

As tags que não possuem semântica não definem um significado para aquele texto, normalmente são utilizadas apenas para fins de separação e estilização. Veja logo abaixo a lista de algumas tags sem semântica:

* `<div>`
* `<span>`
* `<b>`
* `<i>`

### Comentários

Comentários no HTML ou em qualquer outra linguagem são notas que podem ser incluídas no código fonte para descrever o que se quiser. Assim, não modificam o programa executado e servem somente para ajudar a pessoa que está desenvolvendo a melhor organizar os seus códigos. Para comentar algum código no HTML você deve envolvê-lo entre  **<!-- Seu código aqui –>** . Por exemplo:

```
<!-- 

<div>
    <p>Esse código será ignorado pelo navegador</p>
</div>

–>
```

## Continua…

Nesse artigo vimos que o HTML é a principal linguagem de marcação da Web e também a tecnologia mais básica do desenvolvimento front-end, ou seja, o pontapé inicial para criação de estruturas de sites e aplicações web.

E agora que conhecemos um pouco mais sobre a estrutura básica, vamos juntos aprofundar cada vez mais! Abaixo, clique para acessar a continuação da série sobre o HTML e suas tags.

---



## Elementos inline

"Inline" é uma categorização dos elementos do HTML, os elementos inline podem ser exibidos em nível de bloco ou outros elementos inline. Eles ocupam somente a largura de seu conteúdo.

Veja um [exemplo](https://codepen.io/mateushenrique-dev/pen/XWavjoQ):

![Exemplo de elemento inline.](https://www.alura.com.br/artigos/assets/o-que-e-html-suas-tags-parte-2-elementos-inline/imagem1.png)

Como você pode ver logo acima, a tag `a` é um elemento inline, ou seja, ele está ocupando somente o tamanho total do conteúdo, que nesse caso é o texto.

Logo abaixo você pode conferir alguns desses elementos inline:

## `<span>`

Muito parecido com a tag sem semântica `<div>`, porém é um elemento em linha que atua como um container genérico para agrupar conteúdos de texto.

```
<span>Olá, mundo!</span>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/QWMeGNZ).

## `<br>`

Essa tag produz uma quebra de linha em um determinado ponto do documento.

Exemplo de utilização:

```
<span>Olá <br> meu nome <br> é <br> Joãozinho</span>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/XWavjvL).

## `<a>`

É um elemento âncora que define um hiperlink, que vincula páginas web, arquivos, endereços de emails, ligações na mesma página. Essa tag com o atributo `href`, indica o destino do link. Também é possível criar âncoras para textos na mesma página com o `href` informando o `id` do elemento destino.

Exemplo de utilização:

```
<span>Clique <a href="https://www.google.com" target="blank">aqui</a> para ser redirecionado para a página do google.</span>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/wvqVoam).

## `<img>`

Utilizada para colocar imagens no site, deve-se utilizar o atributo src, colocando entre as aspas o link ou caminho do arquivo.

Exemplo de utilização:

```
<img src="https://cuponomia-a.akamaihd.net/img/stores/original/alura-637582521816079946.png" />
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/rNzXWaE?editors=1010).

## `<audio>`

Utilizada para inserir áudios no site, tendo como principais atributos:  **src** , recebendo como valor o link ou diretório do audio, **controls** caso queira que seja possível controlar o áudio, **autoplay** para definir que o áudio de tocar automaticamente quando entrar no site, **type** recebendo como valor o tipo do áudio.

Exemplo de utilização:

```
<audio src="" controls></audio>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/vYJoyNm).

## Continua…

Nesse artigo vimos o que são elementos inline e quais são esses elementos, no próximo capítulo veremos o que é e quais são os elementos block level.

---



## Elementos block level

Os elementos em “nível de bloco” ocupam todo o espaço do seu elemento pai (container).

## `<header>`

Define o cabeçalho da página, geralmente no cabeçalho identificamos o site, com a logo.

![Página de um navegador web, no lado esquerdo está escrito Header, sobre um retângulo roxo.](https://www.alura.com.br/artigos/assets/html-tags-elementos-block-level/img1.png)

## `<main>`

Compreende o conteúdo principal do corpo da página.

![Página de um navegador web, no lado esquerdo está escrito Header, sobre um retângulo roxo, abaixo está escrito Main sobre um grande retângulo vermelho.](https://www.alura.com.br/artigos/assets/html-tags-elementos-block-level/img2.png)

## `<footer>`

Define o final da página ou conteúdo, o rodapé, geralmente colocamos contatos, redes sociais, endereço, informações “institucionais” no geral.

![Página de um navegador web, no lado esquerdo está escrito Header, sobre um retângulo roxo, abaixo está escrito Main sobre um grande retângulo vermelho e um pouco mais abaixo Footer em um pequeno retângulo rosa.](https://www.alura.com.br/artigos/assets/html-tags-elementos-block-level/img3.png)

## `<section>`

Dentro do conteúdo principal, essa tag compreende uma seção da página.

## `<article>`

Inclui um artigo da página, muito utilizado em blogs e páginas de criação de conteúdo, também indica o principal conteúdo de texto da página.

## `<aside>`

Representa uma seção que faz referência a outro conteúdo da página, como uma definição, uma explicação extra, avisos, biografia do autor, ou seja um conteúdo complementar.

## `<nav>`

Contempla o menu de navegação das páginas do site, e dentro inserimos a listas e links com a tag `<a href=””></a>`.

## `<div>`

Assim como as outras tags, também funciona como um container, porém a grande diferença é que a div não tem valor semântico, é apenas uma divisão na página para fins de layout.

## `<p>`

Representa um parágrafo.

## `<h1>, <h2><h6>`

A família de cabeçalhos ou headings, define os **títulos** da página. Esse grupo de elementos possuem um alto valor semântico e uma organização hierárquica, indo de `<h1>` até `<h6>`, sendo o h1 de maior valor semântico e o h6 de menor valor semântico.

![De um lado há seis frases, uma abaixo da outra, todas escritas “Olá Mundo!”, a primeira representa o h1, a segunda o h2, a terceira o h3, a quarta o h4, a quinta o h5 e a sexta o h6. Do outro lado, há linhas de código html, com as tags da família de cabeçalhos, indo do h1 até o h6, todas encapsulando o texto olá mundo.](https://www.alura.com.br/artigos/assets/html-tags-elementos-block-level/img4.png)

## `<hr>`

Essa tag constrói uma linha horizontal entre elementos, representa semanticamente uma quebra de conteúdo.

## `<video>`

Utilizada para inserir vídeos no site, a tag possui atributos como **width** recebendo como valor a largura do vídeo em pixels, **height** recebendo como valor a altura do video em píxeis, caso não for informada esses atributos, será utilizado a largura e altura padrão do vídeo, **controls** (quando presente nos permite controlar o video), **src** recebendo como valor o link ou diretório do arquivo de vídeo.

```
<video src="" controls></video>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/rNzXWza).

## Continua…

Nesse artigo vimos o que são elementos block level e quais são esses elementos, no próximo capítulo veremos quais são os elementos que podemos utilizar para compor um formulário.

---



## Formulário

## `<form>`

Essa tag indica que estamos iniciando um formulário, recebe como principais atributos **method** que recebe como valor o método http que esse formulário irá executar (get, post) e **action** que especifica para onde enviar os dados do formulário quando um formulário é enviado.

```
<form></form>
```

## `<input>`

Um campo para que o usuário possa inserir algum texto, data, número, cor, etc… possui como principais atributos  **type** , que recebe como valor o tipo do input.

```
 <input type="text">
```

## `<textarea>`

Representa uma caixa de texto, útil quando você quer permitir ao usuário informar um texto extenso em formato livre, como um comentário ou formulário de retorno.

```
<textarea></textarea>
```

## `<button>`

Um botão clicável, possui como principais atributos  **type** , que caso receba **submit** como valor e esteja dentro de um formulário, irá submeter o formulário.

```
 <button type="submit">Enviar</button>
```

## `<label>`

A tag label é importante para os campos de formulários. Ela especifica qual o "rótulo" do input (a que se refere o input, como por exemplo envolvê-la em um texto “Nome completo”), e ajuda na experiência do usuário durante a utilização e preenchimento do formulário.

```
<label>Nome completo</label>
```

Veja um [exemplo](https://codepen.io/mateushenrique-dev/pen/oNGgNKE?editors=1010) de formulário criado utilizando as tags que aprendemos:

![Formulário com dois rótulos, no primeiro está escrito Nome Completo, abaixo tem o campo para digitação, mais abaixo está o segundo rótulo Digite seu elogio, seguido de outro campo para digitação, e por último há o botão de Enviar.](https://www.alura.com.br/artigos/assets/o-que-e-html-suas-tags-parte-4-elementos-formulario/imagem1.png)

## Continua...

Nesse artigo vimos quais elementos utilizamos para compor um formulário, no próximo veremos o que são atributos e como utilizá-los.

---



## class=”NomeDaClasse”

Classes são como classificações de uma tag/elemento, para que no CSS estilizar uma tag específica, ou um conjunto de tags. Também é possível usar no [JavaScript](https://www.alura.com.br/artigos/javascript) para selecionar uma tag específica.

HTML:

```
<h1 class="titulo">Mergulhe em Tecnologia!</p>
```

CSS (Não se preocupe com o css, você pode aprendê-lo no curso [HTML5 e CSS3 parte 1: A primeira página da Web](https://www.alura.com.br/curso-online-html5-css3-primeiros-passos)):

```
.titulo {
  font-size: 21px;
  color: #fff;
  background: blue;
}
```

No código acima selecionamos o css com o seletor de classes usando ponto antes do nome da classe (`.classe`), e então aplicamos um tamanho de fonte, cor e cor de fundo.

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/RwLNNLd?editors=1100).

## id=”NomeDoId”

Identificar de forma única um elemento naquela página HTML... É utilizado para identificar destino de âncoras, labels e outras funcionalidades neste sentido.

## src=”Link ou diretório da mídia"

Comumente utilizado para indicar para a tag qual arquivo ou mídia utilizar. Recebe valores como links (`https://google.com/minhaimagem.jpeg`) ou o nome de um arquivo já presente no projeto (`/minhaimagem.jpeg`).

```
<img src="https://www.alura.com.br/assets/img/alura-share.1636535197.png" >
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/OJxPPXe).

## alt=”Texto alternativo”

O atributo alt fornece informações alternativas para uma imagem se um usuário por algum motivo não puder visualizá-la (devido à conexão lenta, um erro no atributo src ou se o usuário usar um leitor de tela).

```
<img src="https://www.alura.com.br/assets/img/alura-share.163653197.png"  alt=”Logo da alura”>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/VwMYYKG).

Obs: A imagem não foi carregada propositalmente para simular um link errado (como nesse caso) ou uma má conexão onde a imagem não venha a carregar.

## href=”Url”

Para a tag `<a>`, o atributo href especifica a URL da página para a qual o link vai.

```
<p>Clique <a href="https://www.alura.com.br/">aqui</a> para ir para o site da alura</p>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/MWEYYJJ).

Para elementos `<link>`, o atributo href especifica a localização (URL) do recurso externo (geralmente um arquivo de folha de estilo).

## lang=”Linguagem”

O atributo lang especifica o idioma do conteúdo da tag.

Os exemplos comuns são "en" para inglês, "es" para espanhol, "fr" para francês e assim por diante.

## target=”blank”

Esse atributo abre o link do documento em uma nova janela ou aba.

```
<p>Clique <a href="https://www.alura.com.br/" target="blank">aqui</a> para ir para o site da alura</p>
```

Veja o [resultado](https://codepen.io/mateushenrique-dev/pen/xxXbbqY).

## Conclusão

Agora é com você!

Encerramos por aqui a nossa série de artigos sobre o que é html e suas tags, vimos desde a estrutura básica até uma explicação detalhada de cada tipo de tag.

Mas essa troca não acaba aqui. Agora, queremos saber de você!

Qual foi a parte dessa série que foi mais interessante para você? Já conhecia todas as tags que foram mencionadas? Teve alguma dúvida durante a leitura?

Você pode responder aqui [nesse tópico](https://cursos.alura.com.br/forum/topico-o-que-e-o-html-e-suas-tags-189126) do fórum, onde também vai conseguir saber mais sobre a opinião de outras pessoas a respeito do HTML e as suas tags.

Além disso, para aprofundar ainda mais, também recomendamos mergulhar os estudos nos cursos da [Formação HTML e CSS](https://cursos.alura.com.br/formacao-html-e-css). Além disso, você pode utilizar os tutoriais do [W3schools](https://www.w3schools.com/html/default.asp) para se guiar no aprendizado das tags.

Bons estudos e até o próximo artigo! =)
