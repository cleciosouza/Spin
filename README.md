Sistema de programação baseado em script visuais converte o script visual em uma linguagem qualquer hoje Spin tem suporte a build para jquery e javascript.

Para o gerenciamento estamos utilizando o http://yeoman.io/

Passos para instalar:
http://yeoman.io/codelab.html

Meus Passos:

1 - Instalar: https://nodejs.org/

2 - Instalar git Windows git: http://creativenotice.com/2013/10/user-yeoman-on-windows-7/:

	1. Download Git from http://git-scm.com/downloads
	2. Run the Git exe and keep the defaults.
	3. When asked about “Adjusting your PATH environment” choose “Run Git form the Windows Command Prompt”
	4. On the next screen, “Choosing the SSH executable“, choose “Use OpenSSH”
	5. On the next screen, “Configuring the line ending conversions“, choose “Checkout Windows-style, commit Unix-style line endings”
	6. Clicking next will start the install process, just let it run.
	7. When the installer completes, just click the “Finish” button. 

3 - Após instalado nodejs e git abra o terminar "cmd" e execute
	
	$ node --version && npm --version 
	$ npm install --global npm@latest
	$ git --version
	$ npm install --global yo bower grunt-cli
	$ yo --version && bower --version && grunt --version
	$ npm install grunt-autoprefixer --save-dev
	$ npm install -g generator-webapp
	
4 - Executando o servidor:

	grunt serve

5 - Executando os testes de unidade:

	$ grunt test

6 - Criando o Build da aplicação:

	$ grunt ou grunt build

7- listas todos os pacotes instalados

	$ bower list

8 - Grava no arquivo bower.js que o pacote foi instalado

	$ bower install respond --save


Criando projeto - Exemplo de como criei o projeto pelo 'cmd':

	$ yo
	escolha a opção 'webapp'
	escolha a opção Bootstrap

	Search Bower's registry for the plug-in we want.
	$ bower search jquery-pjax

	Install it and save it to bower.json
	$ bower install jquery-pjax --save

	If you're not using RequireJS...
	Injects your dependencies into your index.html file.
	$ grunt wiredep

Continuando projeto - Como ajudo a desenvolver ?:

	1 - Clone o repositório
	2 - Entrem na pasta do projeto pelo cmd ou terminal
	3 - Executem os passos "Criando projeto", mas quando pedir para realizar override nos arquivos de configuração ee os index.html ou test.html negue esta ação.
	4 - Execute o projeto e veja esta esta funcionando "grunt serve"

Biografia recomendada:
http://pt.slideshare.net/mateuspadua3/iniciando-com-yeoman-grunt-e-bower?related=1
http://www.infoq.com/br/presentations/desenvolvimento-yeoman#downloadPdf
http://yeoman.io/codelab/setup.html
