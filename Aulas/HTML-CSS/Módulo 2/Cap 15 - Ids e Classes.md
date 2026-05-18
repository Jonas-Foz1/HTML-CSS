
### Usando o id com CSS
- quando temos elementos repetidos no codigo que queremos diferenciar de alguma forma no estilo, usamos um IDENTIFICADOR para cada elemento
- Como fazer: adicionar o parametro ID dentro da tag:
	- ex:  (h1 id="principal")
	- Isso é colocado dentro do codigo HTML
	- No CSS, colocar o seletor:
	- h1#principal {
		- descritores
	- }
	- Pode escrever somente #principal tambem
- Com isso, é possivel personalizar qualquer elemento
- existe tambem o class, que vai ser explorado nas proximas aulas

### Diferenças entre id e class
- o id é limitado no sentido que só pode existir UM elemento com esse id
- ou seja, se eu criar um id para um h1, não posso aplica-lo em outro h1 ou outro elemento
	- na pratica funciona, mas pelas regras da W3C não está correto
- para editar multiplos elementos usando um mesmo seletor personalizado, usamos o CLASS
- Dica - dar nomes as classes de acordo com as funções
- DICA - para editar multiplos elementos ao mesmo tempo, usar ALT + CLIQUE para selecionar multiplas  linhas
- para adicionar essas classes no CSS, usar:
	- ex: class = "basico"
	- .basico {
		- descritores
	- }
- também é possivel aplicar mais de uma classe ao mesmo elemento (não precisa separar com virgula)
- 

### Pseudo Classes
- use a tag DIV para criar linhas preenchidas em toda a pagina
- use a tag Display: inline-block para colocar varias linhas uma do lado da outra
- para criar a PSEUDO CLASSE, usar :
	- relacionado a ESTADO de um determinado elemento
	- ex: div:hover
- é possivel tambem criar pseudoclasses aplicadas a elementos especificos dentro de um seletor:
	- ex: div:hover > p
	- nesse exemplo, está se aplicando descritores especificos para paragrafos dentro de um div, quando se passa o mouse por cima do texto (hover)
	- nesse exmplo, p é um elemento FILHO de DIV
	- isso adiciona camadas de complexidade nas paginas para criar menus e paginas interativas

### Pseudo Elementos
- outra pseudo-classes:
	- a:visited. Determina descritores para links ja acesssados
	- a:active. Determina descritores para links durante o clique do mouse
- para adicionar PSEUDO ELEMENTOS, usar ::
	- relacionado a adicionar coisas a elementos antes ou depois
	- ex: a::after. adicionar após o link

### Resumo
- #' = id
- . = class
- : = pseudo class
- :: = pseudo element
- > = children