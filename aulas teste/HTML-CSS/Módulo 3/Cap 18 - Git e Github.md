
###  O que é Git e Github?
- repositorio local e remoto
	- repositorio é um local onde se guarda coisas
	- existem os feitos no computador proprio e existem os online
- ideal é guardar versoes anteriores dos projetos para nao perder coisas e ter retrabalho
- para fazer isso de forma eficiente, pode usar um gerenciador de versões
- um dos softwares qie fazem isso é o GIT
	- software que mantem versoes de codigos dentro do meu PC
- porém, se acontecer algo com meu PC, tudo que foi salvo no git será perdido
- ou ainda, para permitir que outro usuario acesse seus projetos e codigos de forma pratica
- para isso serve o GITHUB - manter backups na nuvem
- git = repositorio local
- github = repositorio remoto

### Primeiro Repositório no Git e Github no PC
- para repositorio local
	- Criar no github for desktop
	- usar imagem do print como ref
- ![[Pasted image 20260518185916.png|675]]
- o Github vai criar uma serie de arquivos e pastas para organizar o repositorio LOCAL
- depois disso, basta clicar em PUBLISH para subir o repositorio para o github remoto

### Gerenciando Repositórios no Github
- é possivel acessar o repositorio abrindo ele com o CODE na pag inicial
- sempre que houver uma mudança em algum arquivo do repositorio, o github vai sinalizar e perguntar se vc quer subir essa mudança na main (commit to main)
- depois de dar commit em todas as alterações, é possivel fazer um PUSH do repositorio local para o repositorio remoto (PUSH ORIGIN)
- Outra forma de criar repositorios
	- pode criar pastas usando somente o github desktop
- voce pode criar multiplos repositorios, mas só pode visualizar um por vez
- se quiser alterar alguma config do repositorio remoto, abrir no site do github e ir em settings
- para apagar repositorios
	- LOCAL - selecionar repositorio para apagar > repository > remove
	- REMOTO - selecionar repositorio no site > settings > delete this repository


### Hospedando Sites com GitHub Pages
- entrar no repositorio desejado
- Clicar em SETTINGS
- na esquerda, ir em PAGES
- Alterar a branch para MAIN e deixar a pasta como / root
- clicar em save
- em cima, navegar para ACTIONS
- Clicar onde está escrito "pages build and deployment"
- clicar no link abaixo de DEPLOY
- a pagina inicial vai ser o texto do arquivo README do repositorio
- link: https://jonas-foz1.github.io/HTML-CSS/
- para acessar paginas especificas do repositorio, usar o diretorio especifico na barra de busca
- ATENÇÃO - cuidado com Caps LOCK e acentos
- dentro do README, é possivel colocar links usando a tag (a)
- com isso, pode referenciar exercicios ou desafios especificos
- 