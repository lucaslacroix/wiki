<h1 align="center">
    Fazer debugs com Nodemon + Sucrase
</h1>

**1º passo** - Criar um script no **package.json** para que consiga fazer debug com Nodemon + Sucrase

    "scripts": {
        ...,
        "dev:debug": "nodemon --inspect src/server.js"
    }

**2º passo** - No VScode, criar um **launch.json** com as seguintes configurações

    {
        "version": "0.2.0",
        "configurations": [
            {
                "type": "node",
                "request": "attach",
                "name": "Launch Program",
                "restart": true,
                "protocol": "inspector"
            }
        ]
    }
