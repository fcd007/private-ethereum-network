# private-ethereum-network

### Building a private network step by step Blockchain Ethereum with Geth tested

#### Criando uma rede privada Ethereum passo a passo com Geth

Lançada em 2015, Ethereum é a principal blockchain programável do mundo.

###### Rede privada e teste
 
###### Índice
* Construir rede privada
* Testar rede privada
* Transação para testar a rede privada

###### Ambiente
* Linux Ubuntu 20.04 LTS
* Go (version 1.10 or later)
* geth (go-ethereum)

Execute os seguintes passos:

###### Download e instalação geth
Execute o comando `make all` ou `make geth`
Dentro do diretório  go-ethereum
Vá até a pasta `/go-ethereum/build/bin/` pode ver o arquivo geth

###### Inicialize a rede privada
Crie seu arquivo genesis.json execute com 
`touch genesis.json ` ou `nano genesis.json`

Abra a pasta que foi criada para armazenar os dados
`./geth --datadir /home/usuario/armazenamento/ init genesis.json `

Após essa etapa poderá ver duas pastas geth e keystore em sua pasta de armazenamento.

###### Executar rede privada
Execute `./geth --datadir /home/usuario/armazenamento/ --networkid xx console `
