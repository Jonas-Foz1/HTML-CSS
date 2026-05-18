
### Primeiros Passos em Tipografia
- tipografia - surge para melhorar a legibilidade das letras
	- typos = impressao no papel
	- graphia = escrita
- a forma de escrever tambem transmite emoções
- em design, pensam-se em juntar 3 coisas
	- imagens
	- cores
	- letras
- esses são os pilares para criar uma identidade visual e apresentar o conteudo de uma forma que engaja os usuarios
- a forma de escrever uma palavra impacta diretamente na forma como ela é interpretada
- as fontes transmitem emoções tambem

### Anatomia dos Tipos
- Tipo = como desenhar cada uma das letras
- Times New Roman
	- fonte serifada
	- da classe romana
- letra x é o ponto de partida para construção de todas as fontes
	- porque existe uma metrica chamada de "altura x"
- Altura x define a altura base das demais letras da fonte
- a altura das letras maiusculas é diferente - chamada de "altura das maiusculas"
- a altura do "vazamento" das letras tem nomes especifios
	- ascendente - para cima
	- descendente - para baixo
- a soma de todas as juntas é chamada de "corpo"
- esses itens são todos MÉTRICOS
- existem tambem os anatomicos
- itens anatomicos das fontes
	- serifa = pequenos traços que aparecem em algumas letras nas extremidades
		- cria uma linha imaginaria no texto que facilita a leitura das palavras
	- haste = parte reta de uma letra (k, A)
	- filete = une duas hastes ou 1 ou mais hastes e arcos (A, E)
	- arco = curva nas letras (n)
	- esporão = pequeno "pé" que fica na base da letra (b)
	- vertice = ponta de alguma letra (A)
	- terminal = elemento que não está preso em outro lugar (r)
	- braço = elemento que sai de uma haste para cima (k)
	- perna = elemento que sai de uma haste para baixo (k)
	- pé = onde ficam as serifas (A)
	- espinha = curvas das letras (s)
	- barriga = união de 2 arcos (b)
	- olho = buraco na letra fechado de todos os lados (Q, e, b)
	- orelha = pequena ponta na parte de cima ligada ao olho (g)
	- cauda = ponta da parte de  baixo ligada ao olho (g, Q)
- Cada letra de uma fonte é chamada de GLIFO
- conjunto de glifos de uma determinada familia é a FONTE
- algumas fontes de varias formas de representar um mesmo glifo
- o conjunto dessas formas chama-se FAMILIA TIPOGRAFICA
	- light
	- normal
	- seminegrito
	- negrito
	- extranegrito
- A partir disso, surge o conceito de categorias de fontes:
	- serifadas - fontes que tem serifa
	- sans-serif - fontes sem serifa
	- monoespaçadas - todos os glifos (incluindo pontuação) tem a mesma largura
	- handwriting (script, scriptada) - fonte que simula caligrafia humana
	- display (comemorativas) - não possui nenhuma das caracteristicas mencionadas anteriormente

### Familias de Fonte com CSS
- Dentro do HTML / CSS, usa-se o codigo style : font-family para definir a fonte de um texto
	- *IMPORTANTE*: fontes que são espaçadas com 2 nomes (tipo Courier New) precisam ser escritas dentro de aspas simples: 'Courier New'
- Para textos em sites, das preferencia para fontes SANS-SERIF (não serifadas), para facilitar leitura:
	- Arial
	- Verdana
	- Helvetica
- Alguns PCs podem nao ter alguma fonte especifica
- por isso, no font-family, ideal é sempre colocar umas 3 fontes para garantir que o usuario vai conseguir ver o texto
- na duvida, buscar por CSS WEB SAFE FONT COMBINATIONS
	- https://www.w3schools.com/cssref/css_websafe_fonts.php
	- 
- é possivel tambem definir uma categoria de fonte, sem especificar qual, para o PC do usuario definir:
	- sans-serif
	- serif
	- monospace
- usando os estilos internos ou externos, é possivel customizar diferentes fontes para diferentes partes do texto
	- ex: h1, h2 {font-family: serif}

### Tamanhos de fonte
- para definir o tamanho das fontes temos **medidas absolutas** e **medidas relativas**
- Medidas absolutas
	- cm, mm, in, px, pt, pc
	- recomendado = px (pixels)
- Medidas relativas
	- em, ex, rem, vw, vh, %
	- recomendado = em (relativo a letra maiuscula)
- Padrao do CSS é 16px
- 1em = 16px
- a vantagem de usar EM é sempre adaptar o tamanho da fonte ao tamanho da tela do usuario

### Peso, Estilo e Shorthand font
- o peso da fonte é a tag FONT-WEIGHT
- Existem alguns tipos:
	- lighter
	- normal
	- bold
	- bolder
- nem todas as fontes tem todos esses tipos
- outra variação é a numerica
	- começa em 100 e vai até 900
- isso permite editar com mais precisão o peso da fonte
- para cada fonte escolhida, precisa verificar as opções de peso disponiveis
- outra variação possivel é FONT-STYLE
	- Normal ou italic
- TEXT-DECORATION = colocar underline
- é possivel unificar todos essas tags usando a funçao SHORTHAND FONT
	- na ordem: font style > font weight > font size > font family

### Usando Google Fonts
- existe um repositorio gratuito de fontes mantido pelo Google
- https://fonts.google.com
- navegando pelo google fonts, vc pode escolher uma fonte e adicionar ao codigo usando EMBED
- escolher a opção para CSS (@import) e add isso na linha logo abaixo da tag STYLE
- depois de usar o IMPORT, pegar do site tambem o codigo para adicionar os atributos da fonte na pagina
- lembrando que, em CSS, os imports são REGRAS e precisam ser colocados no codigo antes de qualquer outro seletor de estilo, logo no começo do style
- Ordem de escrita do style (interno ou externo):
	- Regras (@import, @charset)
	- Seletores (body, h1, h2, p)
	- Declarações (conjuntos de propriedades e valores: font-family, font-size, color, etc)

### Usando Fontes Baixadas
- voce pode pegar fontes de outros site e baixa-las no pc
- exemplo:? https://www.dafont.com/pt/
- para baixar fontes, ficar atento se elas possuem glifos acentuados
- fontes podem vir no formato ttf ou otf
	- ttf = truetype
	- otf = opentype
	- atualmente, projetos usam mais arquivos otf. então dar preferencia a essas
- no codigo, precisa adicionar uma regra (um seletor especial na verdade) usando @:
	- @font-face {
		- font-family: "Nome da fonte"
		- src: url() format()
		- font-weight
		- font-style
	- }
- Normalmente, para criar sites, cria-se uma pasta separada dentro do projeto só para fontes
	- pasta fonts

### Capturando Fontes de Sites
- visitando sites, é possivel pegar fontes de textos em sites
- usando o plugin Fonts Ninja
- https://chromewebstore.google.com/detail/fonts-ninja/eljapbgkmlngdpckoiiibecpemleclhh
- nao funciona no Opera
- para pegar fontes de imagens, existe o recurso What Font Is
- https://www.whatfontis.com

### Alinhamento de Textos
- existem 3 tipos basicos: esquerda, direita e centro
- no CSS3, alinhamentos sao feitos usando TEXT-ALIGN
- nesse atributo, podemos colocar:
	- left
	- right
	- center
	- justify
- Existe uma propriedade chamada TEXT-INDENT
	- ela define um recuo de tamanho especifico para a primeira linha
	- tamanho em px