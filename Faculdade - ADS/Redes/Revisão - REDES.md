Data: 2023-09-19
#redes

---

# Conteúdo

Redes começou a ser desenvolvida, na guerra fria para evitar os ataques nucleares, eles precisavam de uma forma para conectar entre si, surgindo a ARPANET me 1969, depois ela foi ampliada para as instituições de ensino (ex. Stanford), na ARPANET foi desenvolvido os protocolos TCP/IP para que vários dispositivos diferentes comunicassem entre si, uma marca pode criar diversos dispositivos, mas terá que se comunicar pelo mesmo meio.

> Analogia: tenho vários veículos diferentes, mas eles utilizam os mesmo meios para trafegar, como asfalto, ar e vias maritimas.

Logo após surge o boom das WWW (Word Wide Web), internet sendo acessível a qualquer um.

**ISP -** Provedores de rede (internet)

**Rede -** Ligar componentes para compartilhar recursos. Conjunto de software e hardware
+ Hardware: Computadores, roteadores
+ Softwares: Protocolos

### Modelo OSI
Foi desenvolvido para definir um padrão para os Hardwares conversarem entre si de uma forma padronizada. É uma estrutura coneceitual composta por 7 camadas, elas são organizadas de forma que nenhuma interfira na outra e cada uma tem que ter sua função bem definida. Em cada camada é adicionado um header ao pacote, para informa a origem e destino do determinado pacote

![[Pasted image 20230919231600.png]]

O modelo OSI tem três conceitos fundamentais, sendo eles:
1. Serviços
2. Interfaces
3. Protocolos

**7 camadas:**
- Física* - Através de um meio de comunicação os dados serão transmitidos, por exemplo cabo coaxial ou de fibra, por um meio wirelles como bluetooth e wi-fi. IEEE: Conjunto de padrões para redes sem fio
- Enlace* - Garante a integridade dos dados controla a forma que usamos o meio físico para transmitir os dados. MAC - Responsável pelo controle de acesso
- Rede - Garante que os pacotes irão chegar de forma ordenada. IP: protocolo para definir o endereço que os pacotes serão redirecionados | ICMP: Enviar mensagens de controle de informações (ex. o pacote chegou ao destino ou não)
- Transporte - Responsável pela entrega dos dados, a forma que o pacote vai chegar ao seu destinatário de forma correta. TCP: entrega confiavél e ordenada dos dados | UDP: entrega rápida e não confiavél do dado (não confirma se um pacote chegou ele somente envia sem parar os pacotes) | SCTP: protocolo alternativo que oferece multstreaming
- Sessão - Controla o estabelecimento de sessões do sistema (ex. professor comentou um exemplo de abas de um navegador - funções como autenticação)
- Apresentação - Tradução dos dados, garante que o sistema final irá compreeender a informação. SSL/TLS: Criptografa informações para garantir a segurança como o HTTPs
- Aplicação - Lida com o usuário final, o navegador por exemplo. HTTP: Transferência de páginas | SMTP: enviar e-mails | FTP: Enviar arquivos

#### Camda física:
Transmitir um fluxo de bits, quem irá tratar a forma que os dados serão transmitidos de uma máquina para a outra. Essa trasmissão acontecem por meios físicos das seguintes maneiras:

**Pares trançados:** Par trançado de fios é feito porque dois fios paralelos um ao lado do outro formam uma antena, quando os fios são trançados reduzimos os ruídos pois um os sinais se cancelam ou seja menor a interferência.
Os enlaces podem ser usados nos dois sentidos (enviar e receber) ao mesmo tempo **fullduplex**. Ao contrário os que são usados em qualquer sentido mas somente um de cada vez como uma linha de trem são chamados de **half-duplex**. Uma terceira forma seria em que trafegam os dados somente em uma direção com uma rua de mão única se chama **simplex**.

**Cabo coaxial:** Um único fio de cobre que envia sinais elétricos que são convertidos em bits, eles tem a melhor proteção contra ruídos e interferência, utilizados para enviar sinais de longa distância, começaram a serem usados somente para transmissão de Televisão, depois foram utilizados para enviar pacotes na internet.

**Fibra óptica:** Um cabo de vidro, que em uma ponta é enviado um sinal de luz, e na outra ponta um receptor que irá receber os sinais;

#### Camada de enlace:
Responsavél pela forma que os dados serão acessados/recebidos pelo meio físico, controlar como acessar a mídia, não é possivél enviar vários dados ao mesmo tempo, se fizermos isso teremos colisão (ex. *barramento*).

Essa camada se divide em duas partes, MAC e LLC.
+ MAC (Media Acess Control):
	Responsável por controlar o acesso ao meio físico de transmissão. Principal função e definir em uma rede quem vai enviar para onde e para quem, como endereço de uma casa.
	MAC irá lidar com colisão de dados, para garantir que um dado será enviado de cada vez.
+ LLC (Logical Link Control):
	Localizada acima da subcamada MAC, fornece uma interface de rede entre o MAC (quem controla a forma que os dados são enviados) e que os protocolos da camada acima de rede se comuniquem entre si.

**Modulação:** usar a tensão de dados possitivas para representar bit 1 e uma tensão negativa como um bit 0;
**Demodulação:** compreender os dados;

### Topologia de Rede:
Forma que são organizadas os elementos de uma rede de comunicação. As principais topologias de rede são 6:

![[NetworkTopologies.png]]

**Topologia Anel:** Os componentes ficam ligados em loop fechado, um transmite por vez, não tem colisão, mas se um ponto perde quebra toda a rede
**Topologia Árvore:** Combinação de várias topologias de Estrela, dados transmitidos por niveis de hierarquia.
**Topologia de Estrela:** Todos conectados ao centro (switch ou hub).
**Topologia Híbrida:** Combinação de várias toplogias.
**Topologia de Malha:** Todos os dispositivos são conectados entre si, comum em *datacenter*.
**Topologia Ponto a Ponto:** Dois dispositivos conectados

### Diferença entre Switch e Hub:
Usados em redes LAN para conectador diversos dispositivos ao mesmo ponto (topologia de estrela).

##### Hub:
Ele envia os dados para todas as portas conectadas, tenho 5 equipamentos conectados a um hub, se o equipamento 1 for enviar um dado para o 3 ele vai enviar o pacote para todo mundo. Pouca eficiência pois envia dados atoa e pode causar colisão.

##### Switch:
Um equipamento inteligente, no modelo OSI ele vai atuar na camada 2 (enlace). Ele tem uma tabela com o MAC de cada dispositivo, quando o equipamento 1 quer enviar um dado para o 3 o switch sabe onde que o equipmento 3 está e envia o dado somente para ele. Elimina colisão, pois não envia dados aleatórios para quem não precisa.