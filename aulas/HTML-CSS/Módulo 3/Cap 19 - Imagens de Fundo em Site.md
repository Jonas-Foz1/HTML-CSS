
### Baixando Imagens
- imagens do exercicio 22

### Colocando Imagem de Fundo no Site
- Para colocar uma imagem, usar a Tag:
	- background-image
	- add url(" ")
	- ex: background-image: url("Imagens/pattern001.png");
- isso vai fazer a imagem ser replicada X vezes no fundo, a depender do tamanho
- DICA: vc tambem pode aplicar imagem de fundo no Body todo
- todo elemento visual que funciona como uma caixa pode receber uma imagem de fundo

### Imagens de Fundo que se Repetem
- é possivel colocar URLs externas diretamente na background imae
- também é possivel mudar o tamanho da imagem usando a tag:
	- BACKGROUND-SIZE
- IMPORTANTE: mudar a viewport NAO altera o tamanho da imagem
- repetição das imagems é automatica, mas é possivel customizar isso com a tag:
	- BACKGROUND-REPEAT:
		- repeat
		- no-repeat
		- repeat-x
		- repeat-y

### Configurando Posição de Imagem de Fundo
- para isso, usamos a tag:
	- BACKGROUND-POSITION
		- x: left center right
		- y: top center bottom
		- combinando essas 2 coordenadas, é possivel definir o "ponto de ancoragem" da imagem dentro de cada elemento
- DICA: para imagens colocadas no BODY, é possivel usar:
	- height/width: XXvh (vh é viewport height - define um padrao para o body preencher XX% da viewport)
- O ponto de ancoragem sempre vai definir qqual pedaço da imagem vai ficar fixado quando o tamanho da tela aumentar ou diminuir