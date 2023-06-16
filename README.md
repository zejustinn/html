# HTML (Hyper Text Markup Language/Linguagem de marcação de hipertexto)

O HTML é a linguagem de marcação padrão dos websites. Ele é utilizado para descrever a estrutura das páginas através de uma série de elementos, que são definidos por tags, e que visa informar ao navegador como mostrar o conteúdo da página.

> ATENÇÃO: O HTML é uma tecnologia que básica para a criação de páginas de websites, porém para a criação de um site completo é necessário o utilizar juntamente com outras tecnologias como CSS e JavaScript 🤓 \
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
&emsp;&emsp;...Tags\
&emsp;&emsp;...Elementos\
&emsp;&emsp;...Aninhamento\
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

Os conceitos básicos é a seção de conceitos/informações que _EU_ considero fundamentais para o devido entendimento da tecnologia e que fazem com o que desenvolvedor tenha a consciencia de o que é o que e do real motivo da real necessidade de cada informação

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>

### Editores

Para escrever arquivos HTML qualquer editor de texto serve, desde algo mais robusto como uma [IDE(Integrated development environment/Ambiente de desenvolvimento integrado)](https://aws.amazon.com/pt/what-is/ide/#:~:text=Um%20ambiente%20de%20desenvolvimento%20integrado,uma%20aplica%C3%A7%C3%A3o%20f%C3%A1cil%20de%20usar.) até algo mais simples como o Bloco de notas do seu computador. \
Como o objetivo é entender o HTML aprendo a o utilizar, iremos utilizar o bloco de notas para ajudar a fixar o conhecimento através da escrita dos elementos sem nenhum auxílio.

> ATENÇÃO: A escrita do código HTML pode ser feita com qualquer editor de texto, porém para o código ser interpretado ele deve ser aberto com algum navegor

Passo a passo:

- Abra o menu iniciar
- Digite "Bloco de notas"
- Aperte "enter"
- Escreva algum código HTML
- Selecione salvar o arquivo
  - Aperte em "Arquivo" e então em "Salvar" OU aperte "ctrl + s"(segurar a tecla "ctrl" e apertar a tecla "s")
- Escolha um nome para seu arquivo HTML e adicione ".html" no fim dele. Exemplo: "teste.html" - "teste" foi o nome escolhido e ".html" adicionado no fim
- Selecione o tipo de arquivo como "Todos os arquivos"
- Salve
- clique com o botão direito do mouse e selecione "Abrir com" > seu navegador de preferência

Passo a passo com imagens:

![Menu iniciar](./assets/bloco-de-notas-menu-iniciar.jpg)
![Pesquisar "Bloco de notas"](./assets/bloco-de-notas-menu-iniciar-pesquisar.jpg)
![Abrir opção "Arquivo"](./assets/bloco-de-notas.jpg)
![Selecionar "Salvar"](./assets/bloco-de-notas-salvar.jpg)
![Nomear, selecionar tipo e salvar](./assets/bloco-de-notas-salvar-opcoes.jpg)
![Abrir arquivo com o navegador ](./assets/bloco-de-notas-abrir-com-navegador.jpg)
![Resultado](./assets/bloco-de-notas-resultado.jpg)

> Nota: O passo a passo foi criado em um sistema operacional Windows 11 em outros sistemas operacionais os passos podem varias um pouco porém é sempre muito semelhante

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

<p align="right"><a href="#índice">voltar ao índice ⬆️ </a></p>
