Source: Glauco - UNIP
Project: #project/faculdade 
Areas: #areas/network 
Related: [[Camada OSI]]

---

# Conteúdo

Cada pacote tem um número de enedereço (rota de destino).
<u>Como o rotedor descobre as rotas?</u> Antes do roteador enviar o pacote ele tem que ter uma tabela como a rota/caminhos para o envio de pacotes, tenho que saber o endereço lógico para saber onde enviar o pacote. Cada vez que um pacote vai para outro roteador ele dá um "salto" - Tabelas de rotas são utilizadas para definir qual o próximo salto do pacote - Elas incluem endereço da rede, o próximo endereço do caminho e um custo (calculado por um algoritimo - levado em conta: quantidade de saltos ou número de roteadores até o destino, tiques: tempo, relativa: dinheiro).

**Broadcast:** Envio os pacotes para todo mundo.

**Quantidade de saltos:** ex. unip para santos, anchieta: menos saltos (menor distância) - imigrantes: mais saltos mas talvez o tique (tempo) é menor.

**Métodos para descobrir as rotas (2):**
- Vetor distância: Os roteadores desses tipos, cada um vai construi sua tabela de rota deles e ele vai compartilhar a sua tabela com os outros roteadores ligados a ele, uma relação N para N - muitos para muitos. De tempos em tempos realizo um *broadcast* envio as tabelas para todo mundo atualizando constantemente, trocando a tabela inteira.

- Estado de vinculo: São considerados mais velozes, ele não troca a tabela, ele pega somente a tabela que foi alterada e não atualizando a tabela inteira `> volume de dados` - recebe uma tabela inicial depois faz alterações somente na informação necessária. O roteador somente notifica os outros quando tem alguma alteração. A seleção de rotas pode ser **dinâmica** (roteador escolhe o caminho - usa algoritimos para calcular a rota com menor custo -> quntidade de saltso e custo) ou **estática** (rota fixa, sempre a mesma)

### Serviços de conexão
**LLC:** Controle de fluxo, conexão, erro e ordem -> eles reiniciam a conexão entre os dispositivos. Esse processos são executados entre a comunicação dos roteadores.

**Estrutura do endereço IP:** Conjunto de protocolos define um tipo de endereçamento, inclui um identificador da rede e um identificador do host.
Qualquer dispositivo na minha rede, recebe um endereçamento.
**IP:** um host em 4 byte divididos em duas partes - IPV4 (4 Bytes) | um host de 6 bytes - IPV6 (6 Bytes)
**IPV4**: os dois primeiros conjutos definem endereço sobre a rede, os dois últimos definem sobre o host, os dois últimos conjuntos são únicos. Range de cada conjuto de 0-255, 0 e 255 não são utilizados, 255 para pacotes de *broadcast* (255 - todos broadcast manda para todo mundo).

Cinco classe de endereçamento: A até E -> D (multicast) e E (Reservada) A, B, C usadas para endereçar.
- Classe A: 1-127, identificar o host;
- Classe B: 128-191, identificam a rede;
- Classe C: 192-233, identificam a rede e o último byte o host;
- Classe D: primeiro byte 223-239 usado para pacotes **multicast** (endereçar um host *unicast*, vários hosts *broadcast*, e para grupos de host *multicasts*)
- Classe E: primeiro byte 240-255 usado para test 255.

---

<u>DHCP:</u>  Responsável por gerenciar automaticamente a configuração dos endereçamentos IPs de cada máquina em uma rede. O DHCP pode ser configurado em um servidor ele será responsavél por olhar cada dispositivo que se conectar na rede em questão e definir um IP com base na sua tabela de IP e de outros roteadores e/ou servidores DHCP que compartilharam com ele suas respectivas tabelas. O DHCP também é configurado diretamente no próprio roteador (mais comum de ser utilizado).

<u>DNS:</u> Servidores/Serviços de DNS são responsavéis por definirem um apelido para um IP por exemplo para eu acessar o serviço do [google.com](https://google.com) ele está servindo de apelido para o IP [172.217.17.142](http://172.217.17.142) acessando esse IP você tem acesso a mesma página que o link do google.

<u>Getway:</u> é um dipositivo responsavél para traduzir a comunicação de um dispositivo para o outro, cada máquina/dispositivo interpreta os dados de uma determinada maneira, o *Getway* é responsavél por interpretar as duas pontas, realizando a tradução da mesma, sendo possivél diferentes equipamentos de diferentes máquinas compartilharem dados entre si. Ele pode ser usado para prover uma LAN ou WAN permitindo o acesso a internet (conexão com dispositvos diferentes).