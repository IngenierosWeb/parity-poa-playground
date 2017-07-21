# parity-poa-testnet

Ficheros para la configuración de manera ágil de la testnet.

Con esto arrancamos no solo parity configurado para trabajar con la red , sino adicional-mente un monitor para enviar el estado del nodo al dashboard y poder hacer seguimiento.

### Setup

- Para configurar nodo validador lee ``authority/Run_Authority.md``
- Para configurar nodo cliente lee ``authority/Run_Member.md`` 

### Configuración
El fichero génesis está en `config/chain.json` están agregadas las direcciones validadoras que se han confirmado para que se puedan entender entre los clientes, es importante que todos tengamos exactamente el mismo fichero.

Para que haya sincronía está el fichero `config/bootnodes.list` aquí cualquiera puede poner su propio nodo para que los demás lo encuentren fácilmente.

`monitor.json` controla los parámetros para la monitorización del nodo desde el Dashboard, INSTANCE_NAME es el nombre que se mostrará en el dashboard

###  [ethstats](https://github.com/cubedro/eth-netstats) dashboard.
Hay montado un dashboard en  [http://monlyra.ingenierosweb.co:3000](http://monlyra.ingenierosweb.co:3000) a este dashboard es al que están configurados los nodos para reportar las métricas.