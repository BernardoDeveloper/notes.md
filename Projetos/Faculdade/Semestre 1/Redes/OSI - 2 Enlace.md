Source: Glauco - UNIP
Project: #project/faculdade 
Areas: #areas/network 
Related: [[Camada OSI]]

---

# conteúdo
separada em duas partes *mac* (media acess point) e *llc* (controle de link lógico)

- topologia lógica (camada 2): como os dados trafegam, indepedente da física.

### acesso à mídia
como acesso o cabo, temos que controlar a forma que vamos usar esse cabeamento. temos que definir uma regra

controlar como acessar a mídia, não conseguimos enviar vários dados no mesmo tempo (se fizer isso temos conlisão *ex. barramento*)
- maneira de trafegar

**rede anel**: não tem colisão (envia somente quem tem o token)

podemos definir o controle por disptuta, passagem de símbolos (token) e polling (ambiente industrial)

san (storage area network) - rede para armazenamento -> guardar dados (backup). precisamos de alta velocidade, baixa colisão, alta velocidade, rede anel.

## MAC:
##### disputa
Permite que os dispositvos da rede transmitem quando quiserem, `!colisão`
Retransmissão de dados (enviar algo que já foi enviado), +colisão = +lentidão
Antes de transmitir, eles perguntam ao cabo se alguém está no cabo. Analogia de entrar na auto pista. Protocolo **CSMA** decta se tem alguém utilizando o cabo, *reduz* colisão.

*CSMA*: tenta transmitir para a física (cabo), por exemplo se eu colidir eu falor para a camada superior (rede) não consegui transmitir, a de rede fala pode reenviar, ex. ACK (do TCP)
*CSMA/CD*: ao invés de depender da camada superior para reenviar a informação se colidir ele já percebe e já envia o dado por si mesmo.

##### Passagem de símbolos:
Envio de token, somente enviará o dado quem está com o token. Uma rede deterministica, pois temos uma média de quanto tempo cada um está utilizando token podendo definir, quanto tempo de uso em média, e também podendo definir prioridade `0 colisão`.
Necessita de dispositivos mais inteligentes, para o recebimento e envio de token, necessitam de um equipamento para controlar a detecção e recuperação de falhas.

### Endereçamento:
Equipamentos precisam se identificar dentro da rede. Camada de Link de dados se refere aos dispositvos MAC Adress.
Na camada de enleace adicionamos um **cabeçalho** o endereço MAC.

## LLC

### Serviço de conexão:
Determina o nível para recuperar os erros.
1- Serviços não confirmados, sem conexão: Manda pacotes de A -> B somente envia sem controle de ordem, não confirmo se chegou ou não.
2- Serviços orientados a conexão: controlo fluxo, ordem, tudo, se recebeu ou não o pacote.
3- Serviços confirmados sem conexão: Controlo fluxo erro mas não a ordem.

**LLC:** controlo os erros e fluxos, por mensagens de confirmação

controlar fluxo verifica se o receptor pode receber as infromações.
*Checksums:* Compara os valores