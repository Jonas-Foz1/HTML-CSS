
- CSS podem ser aplicadas de 3 diferentes formas
	- inline
	- internos
	- externos
### CSS Inline
- Estilos feitos na mesma linha HTML
- é o que vc faz adicionando o atributo STYLE dentro das tags
- ex.: style = "color: mediumblue"
- ponto fraco - precisa adicionar estilos para cada titulo, paragrafo, etc
- mas não existe significado - não faz parte da utilidade do HTML
- essa forma da muito trabalho e ainda polui bastante o codigo HTMK
- alem disso, se precisar mudar o estilo geral do site em algum momento, vai precisar mudar cada linha de codigo 1 a 1
- não vai ser utilizado no dia a dia
- metodo para configurações pontuais

### CSS Interno (ou local)
- aplica um estilo de forma separada do conteudo HTML
- dentro do HEAD, pode ser abaixo do titulo, podemos colocar:
	- Tag: Style
	- body {
	- }
- Isso cria um seletor de estilo para a tag body. tudo que for colocado dentro do seletor, será replicado para todo o body
- cada linha que for colocada dentro desses seletores é uma DECLARAÇÃO
- importante colocar ; depois de cada declaração
- você pode criar estilos para h1, h2, paragrafos, etc
- isso cria dois "Blocos" dentro do codigo - 1 para estilo e 1 para conteudo
- essa forma ja pode ser usada bastante no dia a dia para estilos locais de paginas
- Desvantagens
	- estilo ocupa muito mais linhas que conteudo
	- se tiver por ex 30 pag no site, precisa copiar os estilos e colar em todas elas


### CSS Externo
- é a maneira mais versatil de adicionar estilos CSS ao site
- DICA: para criar arquivos no VS CODE, pode escrever o nome, dar ctrl+click e criar arquivo
- para começar:
	- abaixo do titulo, escrever a tag
	- Tag: link:css
	- vai criar uma referencia para uma stylesheet chamada "style.css"
	- usar ctrl+click para criar arquivo
- dentro dessa pagina, colocar todos os seletores de estilo desejados
- IMPORTANTE: precisa criar uma regra dentro da pagina para ajudar na escrita de acentuação
	- @charset "UTF-8";
	- adicionar isso como primeira linha
	- embaixo pode colocar um comentario usando /* e */ - comentario para CSS
	- 
- com isso, cada pagina nova criada pode referenciar a stylesheet usando link
- DICAS: 
	- voce pode usar mais de um link para adicionar mais estilos especificos para a pagina
	- voce pode misturar estilos internos com externos
	- **estilo interno > externo (interno sobrescreve externo)**
	- em termos de prioridade pro HTML: inline > interno > externo