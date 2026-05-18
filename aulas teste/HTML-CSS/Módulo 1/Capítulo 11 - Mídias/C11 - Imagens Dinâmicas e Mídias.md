
### Adaptação de Imagens para múltiplos tamanhos de tela
- existem pessoas que acessam de PC, notebooks, celular e até smart TV
- precisamos adaptar as imagens para multiplos usuarios
- para isso, trabalhamos com multiplas imagens no HTML
- Usando uma ferramenta de imagem, criar templates de imagens pequena, media e grande:
	- P = 200x200
	- M = 700x700
	- G = 1000x1000
- Usar as ferramentas de texto e de pintar cor de fundo para alterar os templates de cada imagem
- exportar cada uma como png para o diretorio que irá acessar essas imagens no VS Code

### Escrevendo o código para adaptar as imagens
- Tag: picture - define a imagem que vai ser colocada no site
	- dentro da tag picture, colocar a tag img e deixar a maior imagem disponivel
- Agora, precisamos adicionar as tags para adaptar as imagens caso a tela do usuario tenha um tamanho menor
- Tag: source:media:type
	- colocar essa tag ACIMA da tag img
- Nos atributos da source, colocar da seguinte forma:
	- media="max-width": XXXpx - por padrão, ele coloca min-width. Fazer a troca para max.
		- DICA: sempre colocar no tamanho 50px a mais que o tamanho da img menor, para considerar barra de rolagem
	- srcset="caminho da imagem menor" - colocar a imagem menor
	- type="image/" - completar colocando o formato da imagem no final. PNG é o padrao
- Para testar, ajuste o tamanho da janela do navegador. A imagem deve mudar a partir do limite definido no codigo
- Para adicionar tamanhos menores, colocar outra linha de source:media:type
- IMPORTANTE - precisa alinhar as sources da MENOR para MAIOR
- Nesse exemplo, a imagem da tag IMG PRECISA SER A MAIOR
- Todos esses ajustes são importantes para melhorar a EXPERIENCIA DO USUARIO
- Melhor experiencia do usuario > mais acessos e menos bounces (saídas) > mais visualização em sites como google

### Inserindo Audios
- as regras de copyright de imagem valem tambem para audio
- tomar cuidado de onde usar audios
- tamanho dos audios tambem impacta muito os sites
- como adicionar audio
	- usar a tag audio
	- adicionar atributos: AUTOPLAY e CONTROLS
- Audios com compatibilidade: MP3, WAV e OGG
- é tambem possivel fazer usando AUDIO + Source:src
	- src="caminho do audio"
	- type="formato" - consultar lista no pdf do cap 11
		- mp3 = "audio/mpeg"
	- vc pode colocar mais de uma source para o navegador ir tentando opções
		- colocar na ordem que  vc quer que ele tente reproduzir
		- se nenhuma opção funcionar, vc pode colocar uma mensagem de erro e colocar o audio para download via link
	- nesse método, precisa adicionar tambem atributos:
		- preload="auto" - só vai considerar que o site terminou de carregar depois de carregar todo o audio
		- preload="metadata" - carrega só alguns dados do audio
		- preload="none" - nao carrega nada previamente
		- controls
		- loop - ficar tocando em loop
	- ATENÇÃO: evitar WAV, pois são muito pesados
	- 

### Formatos de video para site
- para download de videos, podemos usar o PEXELS - https://www.pexels.com/videos/
- para HTML5, os formatos mais suportados são MP4(m4v), Webm, OGV
- ideal é ter varios arquivos de varios formatos nos sites
- para hospedar videos, o programa HandBrake ajuda bastante
	- https://handbrake.fr
- tomar cuidado com qualidade do video
	- no max 1080p

### Videos em hospedagem propria
- para colocar videos no site
- Tag: video
- atributos:
	- controls - coloca o player de video
	- width - muda a largura do video
- a boa pratica é adicionar varios formatos para ser compativel com todos os usuarios
- coloca a tag video
- dentro de video, abre as tags source:src
- adicionar o numero de sources de acordo com o numero de formatos de video desejados
- no atributo TYPE
	- mp4 = video/mp4
	- mkv = video/mkv
	- webm = video/webm
- dentro da tag VIDEO, vc ainda pode colocar
	- width = definir largura
	- controls = painel de controle no inferior do video
	- poster = imagem que vai aparecer quando o video nao for iniciado "thumb"
	- autoplay = atributo para video começar a rodar sozinho (nao parece estar funcionando)
	- loop = reinicia o video automaticamente
- tamanho de video pode escalar consumo de banda com muita facilidade
	- vai consumir muito trafego e ficar caro de hostear
- existe outra forma de hospedar videos que deixa muito mais barato

### Incorporação de Vídeos Externos
- a alternativa é inserir videos usando hospedagens externas, como youtube ou vimeo
- youtube:
	- em qualquer video, clicar em share > incorporate > copy
	- colar isso no codigo do site
	- IMPORTANTE: o youtube só deixa reproduzir videos no site no modo "live server"
		- precisa usar alguma extensao do VS Code para testar (Live Server, Live Preview)
- Vimeo
	- tipo youtube, mas tem opções de deixar video livre ou privado
	- tem uma qualidade melhor de video
	- mas o player dele não é tao bom
	- mesma logica: compartilhar > embed > copy
	- você pode configurar algumas coisas no código
	- o Vimeo nao tem problema pra reproduzir localmente