# Requerimentos mínimos para o funcionamento da aplicação
- RabbitMQ
- MongoDB

Ambos podem ser inicializados de forma simples com o docker utilizando docker-images oficiais disponibilizadas no Docker Hub, ou do jeito que preferir.

As configurações de conexão devem ser informadas no arquivo config.js

```
https://hub.docker.com/_/rabbitmq
https://hub.docker.com/_/mongo
```

# Microserviços de Pedido
Aplicação  contruída em Node.js e Express.js. Estrutura de microserviços utilizando RabbitMQ.

## Instalando serviços
```bash
cd product-service && npm install
cd order-service && npm install
```
Execute o RabbitMQ:

`docker run -p 5672:5672 rabbitmq`

Execute o MongoDB:

`docker run -p 27017:27017 mongo`


## ATENÇÃO: RabbitMQ e MongoDB precisam estar em execução antes de iniciar os serviços.

Para inicializar cada serviço, acesse o diretório e execute:

`npm run dev`

## ALUNOS (RAs)

- Bruna Casagrande R.A: 821121694
- Diego Santos Araujo R.A: 821142329
- Emerson Araújo Rodrigues R.A:821142545
- Lucas Pedrosa Blanco R.A: 821162129
- Matheus Lira R.A:821128518
- Paulo Alef Magalhaes Miranda R.A: 821137880
- Samuel Junior R.A: 821149456
- Stefany Piemontez R.A: 821140092