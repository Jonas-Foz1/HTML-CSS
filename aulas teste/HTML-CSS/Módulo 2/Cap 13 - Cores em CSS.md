### Psicologia das Cores
- o conjunto de cores de um site influencia o interesse do usuario em visitar o site, consumir seu conteudo, comprar seu produto , etc
- são vieses inconscientes que influenciam as decisões dos usuarios
- Por ex, muitas empresas usam azul pois é uma cor associada a calma, tranquilidade, sofisticação. Além de ser uma cor muito "segura" por ser preferencia tanto de homens quanto mulheres em geral
- importante tomar cuidado com contrastes e uso de cores que geram cansaço visual
	- exemplo - fundo preto com letra branca gera muito cansaço
	- para casos onde tem muito texto, focar no padrao - fundo branco e letra preta
- cada cor tem suas caracteristica e aspectos que vão se relacionar com individuos inconscientemente
	- vermelho - fome, paixão
	- amarelo - felicidade
	- verde - saude, natureza, sorte
	- rosa - amor, romance, sinceridade, cuidados
	- marrom - sobriedade, estabilidade, robustez

### Representando Cores com CSS3
- Existem 4 formas de representar cores usando HTML / CSS:
	- 1 - usando os nomes diretos das cores sugeridas pelo código no VS Code
	- 2 - usando códigos hexadecimais
	- 3 - codigos RGB
	- 4 - codigos HSL - hue, saturation, luminosity
- Hexadecimais - cores são representadas por algarismos de 0-9 e letras de A-F
	- cada cor tem um codigo de 6 digitos
		- 2 primeiros são RED
		- 2 proximos GREEN
		- 2 proximos BLUE
- RGB - cores são representadas por quantidades de RED, GREEN e BLUE
	- escala de 0 a 255
	- exemplo: rgb (0,0,255) = AZUL
- HSL - cores representadas por fatores de MATIZ (hue), SATURAÇÃO e LUMINOSITY
	- Hue = valor
	- saturation - 0-100%
	- luminosity - 0-100%
- No VS Code, é possivel mudar manualmente as cores usando o slider de cores ao passar o mouse por cima de uma cor do código
	- clicando na parte superior do slider que aparece, pode trocar entre RGB, Hexadecimal e HSL
	- tem um slider de cor, tom, e transparencia

### Harmonia de Cores
- a base está no circulo cromatico
- o circulo cromatico está focado principalmente na harmonia de cores
- podemos separar ele em cores primarias, secundarias e terciarias
- primarias: amarelo, vermelho e azul
- secundarias (combinações das primarias): laranja, violeta e verde
- terciarias são todas as outras misturas de cores primarias e secundarias
	- nome = primaria + secundaria
	- amarelo-esverdeado, amarelo-alaranjado, vermelho-alaranjado, vermelho-arroxeado, azul-arroxeado e azul-esverdeado
- tambem é possivel dividir as temperaturas das cores
	- frias: azuis e verdes
	- quentes: vermelhas e amarelas
- classificações de harmonia
	- quando for desenvolver um site, é muito importante se preocupar com a paleta de cores
	- a paleta sempre parte de uma cor principal, e depois vai selecionando cores que harmonizam com essa
	- uma paleta tem de 3-5 cores (excluindo preto e branco)
	- Se a marca do cliente for muito importante, a cor do logo normalmente precisa estar na paleta
- Cores complementares
	- cores que mais contrastam entre si - estão em posições opostas no circulo cromatico
	- ex: violeta e amarelo
- Cores analogas
	- cores que não tem contraste tão grande, mas são perceptiveis
	- cores vizinhas / adjacentes no circulo
	- ex: violeta e roxo
- Cores analogas e uma complementar
	- mistura os dois conceitos anteriores
	- ex: violeta, roxo e amarelo
- cores analogas relacionadas
	- cores que são similares, mas geram certo contraste
	- ex: amarelo, laranja e verde
- cores intercaladas
	- parecidas com o tipo anterior, mas tem contraste maior
	- ex: amarelo, laranja, vermelho
- cores triadicas
	- pega uma cor de referencia e pula 3 cores no circulo
	- ex: amarelo, azul, vermelho
- cores em quadrado
	- similar ao anterior, mas pulando 4 cores
- cores tetradicas
	- pega 2 pares de cores complementares
	- ex: verde, vermelho, laranja e azul
- monocromia
	- pega tons diferentes de 1 cor só, mudando saturação e brilho

### Paleta de Cores
- Existem ferramentas que ajudam a criar paleta de cores
- https://color.adobe.com/create/color-wheel
- esse site cria automaticamente paletas de cores com base em uma regra de harmonia e num modo de cor (RGB)
- tambem pode extrair temas de imagens prontas ou documentos
- pode extrair gradientes tambem
- https://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF
- Esse site mostra mais exemplos de preview e como ficaria num site a combinação de cores
- https://coolors.co/403f4c-e84855-f9dc5c-3185fc-efbcd5
- esse cria paletas aleatoriamente a cada click

### Como capturar cores
- jeito mais dificil:
	- tirar print
	- abrir num editor de imagem
	- usar a ferramenta do conta-gotas para pegar a cor
- jeito mais facil:
	- usar a extensão ColorZilla
	- usar o color picker e depois colar o codigo hexadecimal onde desejar

### Como criar degradê com CSS
- para fazer degrade - usamos a função BACKGROUND-IMAGE: LINEAR-GRADIENT
- dentro dessa função, precisa colocar
	- orientação: to right / left ou 90deg
	- cor 1
	- cor 2
	- cor 3...
- Pode colocar TO TOP dentro da direção, mas ai precisa adicionar uma config especial
	- antes do style, colocar um *
	- Isso aplica uma config global a todos os estilos
- O final da tela pode ficar com degrade zuado
	- para arrumar: BACKGROUND ATTACHMENT = FIXED
- Pode mudar tambem de LINEAR para RADIAL GRADIENT
- Pode adicionar tambem % depois de cada cor para definir quantos % da tela cada cor do gradiente vai ocupar
- DICA: não exagerar nos gradientes e cores

### Exemplo pratico - HTML com CSS
- consultar arquivo cor03.html e style.css do exercicio 16
- 