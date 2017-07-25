# parity-poa-testnet

Configuración de un **cliente** de la red con Docker de manera automática incluyendo servicio para la monitorización del mismo con la librería eth-netstats

### Setup
0. Instalar [docker](https://docs.docker.com/engine/installation/) y[docker-compose](https://docs.docker.com/compose/install/)
1. Descarga el repo `git clone https://github.com/IngenierosWeb/parity-poa-testnet && cd parity-poa-testnet/member`
2. Edita el fichero .env y actualiza los parámetros IP con la ip externa del nodo.
3. El fichero config/monitor.json el parametro INSTANCE_NAME debe ser cambiado por un identificador para la red, puede ser cualqueir cadena.
4. `docker-compose up -d`

### Access the Parity UI
0. Ejecuta `docker-compose logs | grep token=` y copia el token de autorización.
1. Accede a http://TUIP:8180
2. Introduce el token de autorización cuando te lo requiera

### Access the [ethstats](https://github.com/cubedro/eth-netstats) dashboard.
Hay montado un dashboard en  [http://monlyra.ingenierosweb.co:3000](http://monlyra.ingenierosweb.co:3000) a este dashboard es al que están configurados los nodos para reportar las métricas.

### Access JSON RPC 
Talk to JSON RPC at [http://127.0.0.1:8545](http://127.0.0.1:8545) with your favorite client.

Be kind and send the poor an ether!