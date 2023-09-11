Data: 2023-09-06
Aula: Camada OSI
#redes

---

# Conteúdo

### Camadas
Aplicação: O pacote a ser transmitido
Aprensentação: Prepara o pacote para ser enviado
Sessão: Garante a comunicação
Transporte: Envia o pacote
Rede: O local que o pacote transita
Enlace: Prepara para transmitir os pacotes
Física: Envia os pacotes de redes por meios físicos. (ex. cabo, wirelless)
### Camada 1 - física
Recebe os dados da camada superior, separar os dados e transformar em bits para fazer a transmissão dos dados. Cria o sinal elétrico.
O que define se será a analogia de 0 ou 1 é a amplitude do sinal elétrico.

Frequencia - eixo x
Amplitude - eixo y

Diversas maneiras para modular o sinal.
Frequência ou fase para enviar os dado -> modem um modulador, transforma um sinal.
**Prova:** modulação

Camada física precisa de um padrão, tempo do sinal.

Largura de banda - quantidade de informação passada em segundo
A informação é o goodput - o restante é ajudantes para a informação chegar ao destino

Cabo ethernet rj45 tem sua conexão somente em duas pontas que são transmitidos a RX e TX o restante é utlizado para redução de ruído.

> O que é: DCE, DTE