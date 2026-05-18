
### Primeiros Passos
- o Modelo de caixas é usado para colocar coisas dentro de outras
	- isso se chama aninhamento
- todo elemento visivel no site é um modelo de caixa
- atraves dessa logica, é possivel editar as caixas usando alguns atributos:
	- height = altura
	- width = largura
	- border = borda
	- padding = acolchoamento da borda pra dentro
	- margin = espaço externo em volta da borda
	- outline = contorno ou traçado, fica em torno da borda

### Tipos de Caixa
- Box level e inline level
- box level sempre se inicia em uma linha nova e ocupa a linha total da tela (largura)
- sempre que a caixa box level for começar, ele vai começar de uma linha "zerada" no conteudo
- inline level não faz esse pulo para proxima linha. ele é criado ao lado do ultimo conteudo e depois permite que o conteudo seja colocado ao lado tambem
- ![[Pasted image 20260430200241.png]]

- a tag DIV por exemplo é um caso de BOX LEVEL
- a tag SPAN é um caso de INLINE LEVEL
- outros exemplos de BOX LEVEL:
	- div
	- h1-h6
	- p
	- main
	- header
	- nav
	- article
	- aside
	- footer
	- form
	- video
- outros exemplos de INLINE LEVEL
	- span
	- a
	- code
	- small
	- strong
	- em
	- sup e sub
	- label
	- button
	- input
	- select

### Modelo de Caixas na Prática
- Usando a função "Inspecionar Elemento" dentro do navegador, já é possivel visualizar o modelo de caixa dentro do dev-tools
- clicando em cima de alguma tag / elemento, é possivel ver varios detalhes sobre as caracteristicas desse elemento
- por ex:
- ![[Pasted image 20260505205521.png]]
- a direita, o "user agent" é o navegador que ta exibindo o conteudo
- outros elementos
	- display: block - padrão de box-level
	- display: inline block - padrão de inline-level
- por esse dev tools, é possivel mudar caractetisticas pagina apenas como "visual"
- essa visão do dev tools é util para testar tags, elementos e ver de forma responsiva alterações nos parametros do codigo
- é possivel editar bordas, margens, padding, cor, etc
- DICA: para descrever margens e paddings, sempre escrever no sentido horario (top>right>bottom>left)
- para colocar elementos de caixa no MEIO DA TELA:
	- Usar MARGIN: auto
- Outiline: fica do lado de fora da borda, colado com ela e dentro da margem
- Como simplificar isso:
	- utilizar shorthands
	- border (largura, estilo e cor)
	- padding (top, right, bottom e left) - se forem todos iguais, basta colocar 1x
		- se colocar 2x, ele espelha cima-baixo e direita-esquerda
	- margin (top, right, bottom e left)
		- se colocar "auto" na direita e esquerda, vai centralizar a caixa
	- outline (largura, estilo, cor)
- é possivel mudar o box sizing usando os comandos
	- height
	- width
- DICA: se quiser mudar rapidamente a propriedade de uma box no DISPLAY:
	- usar o atributo DISPLAY: BLOCK ou INLINE
	- existe tambem o inline-block, que mistura as caracteristicas de ambos

### Grouping Tags
- antigamente, era usado o div para criar varias seções dentro do site
- porem, hoje em dia existem grouping tags semanticas que ajudam a organizar o conteudo
- dá pra organizar um body da seguinte forma:
	- header - cabeçalho
	- nav - links de acesso
	- main - corpo
	- footer - rodapé
	- todos esses são tratados como divs pelo HTML, mas com semantica especifica para ser mais organizado
- Com essas tags agrupadoras, fica facil de criar estilos especificos
- Outras tags agrupadoras
	- Section
	- Article
	- Aside

### Sombras em Caixas
- Cuidado com as sombras - não precisa exagerar
- tag para usar sombras em caixas - BOX-SHADOW
- Ex: box-shadow: 1px 1px 1px black
	- sombra horizontal
	- sombra vertical
	- espalhamento da sombra
	- cor
- é possivel colocar parametros NEGATIVOS para colocar a sombra na orientação oposta
- é possivel visualizar isso tambem no dev tools do navegador
	- depois de editar, só copiar o codigo do dev tools e colar no codigo
- Para deixar as sombras mais suaves, mudar a transparencia da cor para aproximadamente metade ou menor

### Bordas arredondadas
- usar a tag BORDER-RADIUS
- colocando em pixels, é possiveis deixar cantos arredondados ou até deixar a forma circukar
- dá pra personalizar cada canto da borda, ou fazer no padrão 2:2
- tambem pode usar % para alterar as bordas
- 50% = circular

