
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
- Como rodar o site do DESAFIO 10
	- Ir na pasta do desafio
	- copiar os arquivos do site (pastas e arquivo .html)
	- no github, criar novo repositorio
	- deixar ele publico
	- na pasta criada pelo github, colar os arquivos do site
	- renomear o .html para index.html
	- no Github online, fazer o processo de criar o site dos passos anteriores
	- https://jonas-foz1.github.io/projeto-android/
	- esse link pode ser compartilhado com qualquer usuario em qualqquer dispositivo
	- tambem pode criar um QR code desse link em algum QR code generator
	- LIMITAÇÃO - GitHub pages só serve para HTML, CSS e JAVASCRIPT
		- caso queira adicionar algo alem disso, precisa pagar

# Manutenção de sites no GitHub
- no futuro, vamos ver que não é correto mexer na branch MAIN / MASTER
- sempre que precisar ajustar algum site, seguir o seguinte passo a passo:
	- abrir github desktop
	- ir no repositorio do site
	- abrir o codigo com code e a pasta com explorer
	- ajustar o codigo - verificar se a alteração ja está feita no local
	- confirmado o ajuste, fazer o commit dos ajustes no github
	- fazer o push para o site no ar pelo github desktop
- no github desktop, é possivel ver o que foi apagado e adicionado

### Recursos Sociais do GitHub
- é possivel buscar pessoas e repositorios na aba principal do GitHub
- pode seguir repositorio, acompanhar, favoritar, fork, etc
- em um repositorio, é possivel abrir um Issue, ver issues antigos, issues em aberto

### Clonando Repositórios
- em qualquer repositorio, basta clicar no botao verde e depois abrir usando github desktop ou baixar o ZIP
- se abrir com github, basta selecionar diretorio onde vai salvar o repositorio
- clonagem vai ser feita
- com isso é possivel abrir os codigos usando code e ver tudo

### Github em varios PCs
- se estiver fora do meu PC, como faria para trabalhar com GitHub?
- pre requisitos
	- navegador
	- VS Code
	- Git e Github desktop
- logar no github desktop para acessar seus repositorios
- escolher o repositorio para trabalhar e clonar
- salvar em um diretorio especifico
- abrir com VS Code
- com isso, ja é possivel fazer alterações, commits e push
- para deslogar, remover o repositorio local
- dar sign out no github
- apagar as infos do git
- limpar a lixeira
- DICA: para deixar o github mais seguro, buscar algum video com instruções de 2FA, medidas de segurança, etc