<h1 align="center">
    Iniciar servidor com Nodemon + sucrase
</h1>

**1º passo** criar um script no **package.json** para iniciar o servidor em desenvolvimento

    "scripts": {
        "dev": "nodemon src/server.js"
    }

**2º passo** criar um arquivo **nodemon.json** na raiz do projeto e setar as seguintes propriedades.

    {
        "execMap": {
            "js": "node -r sucrase/register"
        }
    }

então basta executar o comando

    yarn dev