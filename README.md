# HTML (Hyper Text Markup Language/Linguagem de marcação de hipertexto)

O HTML é a linguagem de marcação padrão dos websites. Ele é utilizado para descrever a estrutura das páginas através de uma série de elementos, que são definidos por tags, e que visa informar ao navegador como mostrar o conteúdo da página.

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

- [doctype](#doctype)
- [html](#html)
- [head](#head)
- [body](#body)

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
