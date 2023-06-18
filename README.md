# HTML (Hyper Text Markup Language/Linguagem de marcação de hipertexto)

O HTML é a linguagem de marcação padrão dos websites. Ele é utilizado para descrever a estrutura das páginas através de uma série de elementos, que são definidos por tags, e que visa informar ao navegador como mostrar o conteúdo da página.

> Atenção: O HTML é uma tecnologia que básica para a criação de páginas de websites, porém para a criação de um site completo é necessário o utilizar juntamente com outras tecnologias como CSS e JavaScript 🤓 \
> Mas tenha calma "Não dá para ter o resultado sem viver todo o processo. Não apresse as coisas, viva um passo de cada vez." 🧘

> Arquivo: index.html

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8" />
    <title>Título da página do site</title>
  </head>
  <body>
    <h1>Titulo principal da página</h1>
    <p>Um parágrado simples relacionado ao conteúdo do website</p>
  </body>
</html>
```

> Resultado do arquivo acima aberto no navegador

![Resultado do código interpretado pelo navegador](./assets/basic-html-sample-code.jpg)

## Índice

<details>
  <summary><a href="#conceitos-básicos">Conceitos básicos</a></summary>

&emsp;&emsp;[Editores](#editores)\
&emsp;&emsp;[Tags](#tags)\
&emsp;&emsp;...Aninhamento\
&emsp;&emsp;[Elementos](#elementos)\
&emsp;&emsp;...Atributos\
&emsp;&emsp;...Semântica\
&emsp;&emsp;...Espaço ocupado pelos elementos\
&emsp;&emsp;...Entidades HTML\
&emsp;&emsp;...Conjunto de caracteres

</details>

<details>
  <summary>Estrutura básica</summary>

&emsp;&emsp;[doctype](#doctype) \
&emsp;&emsp;[html](#html) \
&emsp;&emsp;[head](#head) \
&emsp;&emsp;[body](#body)

</details>

<details>
  <summary>Tags, suas utilidades e exemplos</summary>

&emsp;&emsp;...em progresso

</details>

<details>
  <summary>Curiosidades</summary>

&emsp;&emsp;...em progresso

</details>

<a href="#referências">Referências</a>

## Conceitos básicos

Os conceitos básicos é a seção de conceitos/informações que _EU_ considero fundamentais para o devido entendimento da tecnologia e que fazem com o que desenvolvedor tenha a consciencia de o que é o que e da real necessidade de cada informação

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### Editores

Para escrever arquivos HTML qualquer editor de texto serve, desde algo mais simples como o bloco de notas até algo mais robusto como uma [IDE(Integrated development environment/Ambiente de desenvolvimento integrado)](https://aws.amazon.com/pt/what-is/ide/#:~:text=Um%20ambiente%20de%20desenvolvimento%20integrado,uma%20aplica%C3%A7%C3%A3o%20f%C3%A1cil%20de%20usar.) que auxilia o desenvolvedor de diversas maneiras diferentes

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### Tags

As tag funcionam como etiquetas que descrevem como o conteúdo deve ser interpretado pelo navegador. As tags possuem duas formas:

- Com fechamento: Nesse formato ela funciona como um container e é sempre utilizada em pares, no qual a primeira tag é a de abertura a segunda tag é a de fechamento e o conteúdo do qual ela descreve se encontra entre elas

```html
<p>Conteúdo</p>
```

> Nota: A tag de abertura nesse exemplo é &lt;p&gt; e a tag de fechamento é &lt;/p&gt;. A tag de fechamento sempre será igual a tag de abertura porém com / nela

- Sem fechamento: Nesse caso a tag não funciona como um container possuindo um conteúdo. Ela tem a finalidade de ser o próprio conteúdo e descrever a si mesma

```html
<img href="./somefile.jpg" />
```

> Nota: Não é necessário o / no final de tags sem fechamento. Porém muitos desenvolvedores utilizam como boa prática

> Atenção: As tags não fazem diferenciação entre maiúsculas e minúsculas, ou seja, a tag &lt;P&gt; e &lt;p&gt; significam a mesma coisa

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### Elementos

Um elemento HTML é um conceito um pouco abstrato, porém simples, mas mesmo assim deve ser entendido com cuidado. Os elementos HTML também possuem duas formas e tem relação direta com as tags:

- Elemento simples: É definido por suas Tags(com fechamento) e tudo entre elas, ou seja o elemento em si É a tag de abrtura, o conteúdo e a tag de fechamento

```html
<!-- Exemplo de elemento simples -->
<p>Conteúdo</p>
```

> Nota: &lt;p&gt;Conteúdo&lt;/p&gt; é um elemento

```html
<!-- Outro exemplo de elemento simples -->
<body>
  <h1>Título</h1>
  <p>Parágrafo</p>
</body>
```

> Nota: &lt;body&gt;...&lt;/body&gt; é um elemento que possue mais dois elementos dentro &lt;h1&gt;Título&lt;/h1&gt; e &lt;p&gt;Parágrafo&lt;/p&gt;

- Elemento vazio: É o elemento definido por uma tag sem fechamento da qual a tag tem a finalidade de ser o próprio conteúdo

```html
<!-- Exemplo de elemento vazio -->
<img href="./somefile.jpg" />
```

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

## Estrutura básica

### doctype

Todos os arquivos HTML devem iniciar com &lt;!DOCTYPE&gt;. \
Essa declaração não é uma tag HTML. Ela na verdade funciona como uma "informação" para o navegador sobre o tipo esperado do documento. \
No HTML 5 a declaração do &lt;!DOCTYPE&gt; é simples:

```html
<!DOCTYPE html>
```

> Nota: A declaração do &lt;!DOCTYPE&gt; Não diferencia maiúsculas de minúsculas

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### html

A tag &lt;html&gt; representa a raiz de um documento HTML. Ela funcionar como um container no qual **TODOS** outros elementos HTML dever ir dentro (exceto a declaração do &lt;!DOCTYPE&gt;).

```html
<!DOCTYPE html>
<html lang="pt-br">
  ...qualquer outro elemento HTML
</html>
```

> Nota: Você deve sempre incluir o atributo "lang" dento da tag &lt;html&gt;, para que o navegador entenda a linguagem da página. Isso se destina a ajudar os motores de busca e navegadores

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### head

A tag &lt;head&gt; é um container para metadados(dados relacionados a dados) e é colocada dentro do &lt;html&gt; e ao lado de &lt;body&gt;. \
Os metadados normalmente descrevem o titulo do página, o conjunto de caracteres, folhas de estilo, scripts, e outras informações dos dados.

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    ...tags HTML de metadados
  </head>
</html>
```

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### body

O elemento &lt;body&gt; contém todos conteúdo mostrado na página, como títulos, parágrafos, imagens, hiperlinks, tabelas, listas, etc.

```html
<!DOCTYPE html>
<html lang="pt-br">
  <body>
    ...Any other HTML content tag
  </body>
</html>
```

> Nota: Pode haver apenas um elemento &lt;body&gt; no arquivo HTML

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

## Referências

- [w3schools](https://www.w3schools.com/html/default.asp)
- [betrybe](https://blog.betrybe.com/desenvolvimento-web/comandos-e-tags-html/)

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>
