Notes:
- [[Camada OSI]]

Source: Glauco - UNIP
Project: #project/faculdade 
Areas: #areas/network 
Related: [[Redes]]

---

# Conteúdo
**Descober de rota:**
Cada pacote tem um número de enedereço.

<u>Como o rotedor descobre as rotas?</u> Antes do pacote enviar o pacote ele tem que ter uma tabela como a rota/caminhos para o envio de pacotes, tenho que saber o endereço lógico para saber onde enviar o pacote. Cada vez que um pacote vai para outro roteador ele dá um "salto" - Tabelas de rotas são utilizadas para definir qual o próximo salto do pacote - Elas incluem endereço da rede, o próximo endereço do caminho e um custo (calculado por um algoritimo - levado em conta: quantidade de saltos ou número de roteadores até o destino, tiques: tempo, relativa: dinheiro).

**Broadcast:** Envio os pacotes para todo mundo.

**Quantidade de saltos:** ex. unip para santos, anchieta: menos saltos (menor distância) - imigrantes: mais saltos mas talvez o tique (tempo) é menor.

**Métodos para descobrir as rotas (2):**
- Vetor distância: Os roteadores desses tipos, cada um vai construi sua tabela de rota deles e ele vai compartilhar a sua tabela com os outros roteadores ligados a ele, uma relação N para N - muitos para muitos. De tempos em tempos realizo um *broadcast* envio as tabelas para todo mundo atualizando constantemente, trocando a tabela inteira.

- Estado de vinculo: São considerados mais velozes, ele não troca a tabela, ele pega somente a tabela que foi alterada e não atualizando a tabela inteira `> volume de dados` - recebe uma tabela inicial depois faz alteraççoes somente na informação necessária. O roteador somente notifica os outros quando tem alguma alteração. A seleção de rotas pode ser **dinâmica** (roteador escolhe o caminho - usa algoritimos para calcular a rota com menor custo -> quntidade de saltso e custo) ou **estática** (rota fixa, sempre a mesma)

### Serviços de conexão
**LLC:** Controle de fluxo, conexão, erro e ordem -> eles reiniciam a conexão entre os dispositivos. Esse processos são executados entre a comunicação dos roteadores.

**Estrutura do endereço IP:** Conjunto de protocolos define um tipo de endereçamento, inclui um identificador da rede e um identificador do host.
Qualquer dispositivo na miha rede, recebe um endereçamento.
**IP:** um host em 4 byte divididos em duas partes - IPV4 (4 Bytes) | um host de 6 bytes - IPV6 (6 Bytes)
**IPV4**: os dois primeiros cojutos definem edereço sobre rede, os dois ultimos defiem sobre o host, os dois últimos conjuntos são únicos. Range de cada cojuto de 0-255, 0 e 255 não são utilizados, 255 para pacotes de *broadcast* (255 - todos broadcast manda para todo mundo).

Cinco classe de endereçamento: A até E -> D (multicast) e E (Reservada) A, B, C usadas para endereçar.
- Classe A: 1-127, identificar o host;
- Classe B: 128-191, identificam a rede;
- Classe C: 192-233, identificam a rede e o último byte o host;
- Classe D: primeiro byte 223-239 usado para pacotes **multicast** (endereçar um host *unicast*, vários hosts *broadcast*, e para grupos de host *multicasts*)
- Classe E: primeiro byte 240-255 usado para test 255.

---

192.168.0.1 - Classe C os três conjuntos iniciais, rede
Maskara (estudar sobre): 255.255.255.255 (padrão) - 
DCHP
DNS
Getway