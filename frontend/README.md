
# TESTER FRONTEND #
a space for testing all about frontend.



# FRONTEND INSTALATION :: STEP BY STEP #

# 00 :: install platforms
- install npm
- install vscode

# 01 :: npm
npm init -y
- inicia o projeto com declarativas básicas

# 02 :: dependencies
- npm i --save-dev webpack webpack-dev-server react react-dom redux react-redux babel-core babel-plugin-transform-object-rest-spread babel-loader babel-preset-react babel-preset-es2015 json-server extract-text-webpack-plugin css-loader style-loader sass-loader node-sass

webpack									// Faz o build de toda a aplicacao (bundle JS CSS)
webpack-dev-server			// servidor webpack
react										// core do React (framwork)
react-dom								// monta o DOM (usar no index da aplicacao)
redux										// core do Redux (framework)
react-redux							// interface entre react e redux
babel-core							// core do Babel (transpiler de ES6 para JS antigo)
babel-loader						// interface entre webpack e babel-core
babel-preset-react			// interface entre react e babel-core
babel-preset-es2015			// interpreta sintaxe ES2015 para JS dos browsers
babel-plugin-transform-object-rest-spread		// interpreta Object Rest Spread (...)
json-server							// permite criar fake API REST com unico JSON.
css-loader							// adiciona o CSS no React (usar c/ style-loader)
style-loader						// adiciona o CSS no DOM (user c/ css-loader)
sass-loader							// converte o SASS para CSS
node-sass								// dependencia do sass-loader
extract-text-webpack-plugin		// interpretador de textos CSS

# 03 :: git ignore
.gitignore
	node_modules
	*.log

# 04 :: configure package.json
"main": "index.js",
"scripts": { "dev": "webpack-dev-server --progress --colors --inline --hot" },

# 05 :: configure webpack.config.js
const webpack = require('webpack')
module.exports = { ... }
- ver arquivos de exemplo com atributos para configurar.