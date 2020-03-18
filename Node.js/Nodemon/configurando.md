<h1 align="center">
    Iniciar servidor com Nodemon
</h1>

Para iniciar o servidor com nodemon basta executar o comando

    nodemon src/server.js

com o nodemon instalado.

Podemos também criar um script no **package.json** para iniciar o servidor sem ter que lembrar esse comando para sempre

    "scripts": {
        "dev": "nodemon src/server.js"
    }

e então basta executar o comando

    yarn dev