
### Planejando a Estrutura
- existe uma ferramenta de planejamento de site
- layout:
	- https://mockflow.com
	- essa ferramenta é usada para criar um draft do site
	- colocando as formas, é possivel visualizar como vai ficar o final
- cores:
	- adobe colors
	- é possivel escolher uma cor base e criar uma paleta a partir dela
- fontes
	- usar google fontes e DaFont

### Transformando layout em código
- layout usado em desafiocompleto.html
- header
- nav
- main
	- article
		- aside
- footer

### Organizando o Conteúdo
- usando ctrl + shift + p, envelopar textos com tags para estruturar textos
- boa pratica visual - colocar sempre as tags na seguinte estrutura:
	- tag
		- conteudo
	- /tag
- usar alt + clique para selecionar multiplas linhas para envelopar varias linhas juntas

### Criando Variaveis em CSS
- dentro da folha de estilo do CSS, criar uma pseudo-classe chamada ROOT
	- :root {}
- para criar uma variavel, usar o prefixo --[nome da variavel]
	- ex: --cor0: #c5ebd6 
	- define essa cor hex como cor0, que pode ser facilmente acessada em qualquer lugar da pagina de CSS
- nos descritores CSS, vai ficar como:
	- color: var(--cor0);
- Outro exemplo, dessa vez com fonte:
	- --fonte-android: "Android", monospace
	- cria uma variavel de fonte apra ser usada
- cores e fontes são boas ideias de variaveis para fazer a manutenção / atualização de sites mais eficiente e pratica
- para deixar as coisas mais clean, criar um seletor global que ajusta o layout de todos os elementos:
	- * {
		- margin: 0px
		- padding: 0px
	- }

### Responsividade para Sites
- é adaptar tamanho e conteudo do site a tamanhos de telas diferentes
- um dos recursos é limitar tamanho minimo e maximo de uma interface
- um parametro ideal é no maximo de 1200px de largura, para nao criar dificuldade de leitura
- para isso, vamos limitar largura maxima e minima
- Instalar a seguinte extensão: WINDOW RESIZER
	- com ele vc consegue ver seu site em diferentes tamanhos de tela
- se eu colocar uma width fixa para alguma box, ela vai "quebrar" inteira quando eu reduzir a tela para menos que aquela width
- quando eu aumentar a tela, eu posso usar MARGIN: AUTO para centralizar a box e nao prejudicar o conteudo
- como fazer de uma forma flexivel:
	- usar MIN-WIDTH e MAX-WIDTH
	- com isso, os conteudos da box vao se adaptar
	- no entanto, isso NAO FUNCIONA para img e video
- para imagem:
	- usar IMG {
		- width: 100%
	- }
	- esse é o jeito mais facil, para ajustar a imagem proporcionalmente
	- mas tem um segundo caminho
- imagem estilo 2:
	- no codigo HTML
	- abrir uma tag picture
	- colocar SOURCE:MEDIA:TYPE
		- Source: caminho da imagem MENOR
		- media: colocar MAX-WIDTH (trocar min-width)
		- type: formato da img
	- logo abaixo, colocar a tag IMG: imagem MAIOR
	- isso vai criar um efeito que, com a pagina até certo MAX-WIDTH, vai usar a img menor
	- a partir dessa MAX-WIDTH, troca para imagem maior
	- ex: pagina responsivo.html

### Responsividade na Pratica
- primeiro ajuste: colocar min-width e max-width no main
- depois: colocar margin:auto para centralizar box
- proximo passo - ajustar imagens
- jeito 1:
	- main img {} - ajusta todas as imagens DESCENDENTES do main
	- width: 100% - imagens vao se adaptar proporcional ao tamanho da box main
	- problema: algumas imagens podem ficar grandes demais  ou pequenas demais em algumas telas
- jeito 2: (para solucionar problemas anteriores)
	-no HTML, envelopar imagens com a tag PICTURE
	- adicionar tag SOURCE:MEDIA:TYPE
	- colocar max-width: tamanho da maior imagem
- DICA: imagens que tem resolução muito baixa, usar CLASS no HTML e no CSS especificar 
	- width: 50% ou menor
	- display: block (img por padrao é tratado como inline no CSS)
	- margin: auto
	- isso ajusta imagens poara nao ficarem "esticadas" no site

### Configurando Header e Menu
- para header:
	- min-height
	- text-align: center
	- padding-top
- para h1 no header:
	- fonte destaque
	- margin bottom
	- font size maior
- para p no header
	- fonte padrao
	- max-width
	- margin auto (precisa colocar isso pois o max-width transforma o texto num bloco box level)
	- padding-right
	- padding-left
- para colocar degrade:
	- trocar background color por background image - linear gradient
		- to bottom
		- cor 1
		- cor 2
		- cor 3
- para menu
	- padding
	- box shadow
- para links do menu
	- border radius
	- padding
	- text decoration none
	- transition duration (DETERMINA UM FADE PARA QUANDO FIZER O HOVER)
	- para a:hover
		- background color
		- color

### Melhorando Formato do Conteudo
- paragrafos
	- colocar margin superior e inferior
	- text align justify
	- text-indent
	- line-height (espaçamento entre linhas) 2em
		- faz isso para evitar o leitor "se perder" no texto
	- font-size 1em
- Strong
	- color
	- font-weight bold
- Links
	- color
	- underline
	- bold
- H2
	- colocar background image - linear - cor01 - TRANSPARENT

### Rodapé, Conteudo Periférico e Links
- Conteudo periferico (aside)
	- backgorund color
	- padding
	- border radius
- para a lista:
	- list-style-type: "\2714\00A0\00A0"
		- 2714 - codigo do emoji do "Check"
		- 00A0 - codigo para um "espaço" no texto
		- NAO É compativel com todo tipo de navegador
	- list-style-position: inside - deixa os indicadores da lista para dentro do texto
	- columns: 2 - quebra a lista em 2 colunas
- H3
	- DICA: usar MARGIN com valores negativos
	- isso faz a margem crescer para o sentido oposto
	- border-radius somente na parte de cima, para "fingir" que o aside é um bloco unico
- Icone no link externo
	- criar uma classe .externo
	- colocar um descritor da seguite forma: a.externo::after {}
		- content: "\00A0\1F517" - icone do link

### Tornando um Video Responsivo
- o problema do video é o embed do Youtube que ja vem fixado
- complica bastante os ajustes
- tem uma "gambiarra" para centralizar os videos do youtube
- passos
	- criar uma div só para videos (usar classe ".video")
	- colcoar margins negativas esq e dir
	- colocar padding
- para centralizar video:
	- criar div.video > iframe {}
	- position: absolute
	- fazer os ajustes descritos no CSS
