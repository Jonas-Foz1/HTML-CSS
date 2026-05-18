- Links são fundamentais para construção de sites
- todo link que é clicavel dentro de uma pagina html é chamado de ANCORA
- o algoritmo do google é baseado em links
### Ancora
- Tag: A (anchor)
- quando colcoar a tag no codigo, precisa indicar a URL dentro do atributo href
- Por padrão, a ancora vai levar para o link carregando a nova pagina dentro da mesma aba
- Se o link for para um site externo, é interessante mudar isso para abrir o link em uma nova pagina
- para fazer isso: incluir o parametro TARGET="_blank"
- para manter abrindo na mesma pagina (padrao): TARGET="_self"

### Link local ou externo
- é possivel tambem adicionar o atributo REL para indicar se o link é local (interno) ou externo
- Local: rel="next"
- Externo: rel="external"

### Linguagem
- existe tambem o atributo HREFLANG
- ele serve para indicar o idioma principal do site para onde o link está levando
- exemplo: hreflang="en" - indica que o site está em ingles
- isso serve para ajudar navegadores que traduzem paginas automaticamente

### Links internos
- para usar links internos, precisamos ter mais de uma pagina no site
- ao criar uma pagina nova, podemos indicar o link intertno na ancora usando somente o caminho da pagina nova
- no VS Code - pode usar ctrl + espaço e selecionar a pagina nova
- dentro das ancoras, podemos usar os atributos rel=NEXT e rel=PREV para indicar como as paginas se relacionam
	- rel="next"
	- rel="prev"
- isso ajuda o google a entender quais são as primeiras e proximas paginas
- Tambem temos a rel=nofollow, que é usada para conteudos patrocinados ou sites que não temos o aval do conteudo
- IMPORTANTE: quando for indicar o caminho de links internos, precisa incluir no caminho todas as subpastas até chegar na pagina de fato
	- olhar exemplo da pagina 003 no ex010
- IMPORTANTE: quando você estiver dentro de uma subpasta e quiser voltar para a pasta principal usando ancoras, precisa usar comandos do LINUX:
	- ./ = a propria pasta atual
	- ../ = voltar para pasta anterior

### Links para download
- usando links, podemos colocar links para download tambem
- DICA: quando estiver criando links, pode colocar "#" como placeholder
- para configurar o link como um download, precisa adicionar o parametro TYPE
	- para PDF: type="application/pdf"
	- para ZIP: type="application/zip"
	- para consultar outros tipo de arquivo - https://www.iana.org/assignments/media-types/media-types.xhtml
- Adicionar tambem o parametro DOWNLOAD "nome do arquivo.formato"
- olhar exemplos no ex010

### Desafios
- fazer desafios d005 e d006 do material
- 
