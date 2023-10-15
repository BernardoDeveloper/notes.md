Source: Glauco - UNIP
Project: #project/faculdade
Areas: #areas/network
Related: [[Camada OSI]]

---

## Sessão
Facilita as comunicações entre quem requisitou e provedor.
3 endereços para enviar um pacote: IP, MAC, porta -> posso acessar diversas janelas de um mesmo provedor, terei o mesmo IP, MAC e porta mas como diferencio se quero acessar determinado conteúdo em um aba e outro em outra vindo do mesmo provedor = *endereço de sessão* para saber qual pacote enviar para cada sessão.

**Administrar sessão:** estabeleço uma conexão -> transfiro os dados (mensagem se recebeu ou não) -> encerro a conexão
- Eu combino a conexão entre o cliente e servidor;

Trabalhando em duas máquinas: load balancer ou um funciona e o outro não;
*Liberação de conexão:* Reconhecer a transferencia retorno de mensagem, para enviar ou não;

## Apresentação
Traduz o que está na camada *sessão* para o *aplicativo*, um formato comum para os dois lados - ele funciona como um tradutor.
- Comprime, criptografa e descriptografa dos dados - faz a conversão dos dados -> ordem dos bit, bytes, caracteres, sintaxe de arquivos;

**Conversão:** Diferentes hardwares trabalham com dados diferentes, um tradutor que entende os dois lados:
- Ordens de Bits: os dados enviam os dados por uma ordem de bits;
- Pode alterar o tamanho de um byte: uma máquina 16 bits consegue comunicar com um de 32 bits eu só preciso na apresentação quebrar a quantidade de bytes, caso seja enviado de 32 para a de 16 por exemplo.
- Alguns sistemas leem os dados de trás para ferente outros ao inverso. Convertendo o esquema de bits do transmissor para o formato do receptor;

---

#### Criptografia
Lá trás não era utilizados sistemas de criptografia como o FTP posso utilizar um sniffer por exemplo como um Wireshark eu consigo ver os dados e pacotes quee stão sendo transmitidos;
Utilizamos um código pré-definido para poder embaralhar os dados, ela pode ser feita por hardware ou por software;
Receptor e Emissor devem conhecer o algoritmo de criptografia;
Código pode ser estabelecido por *Hardware* ou *Software*;
**Conceito dupla cutódia:** uma senha de administrador está uma parte com uma pessoa e outra parte com outra pessoa - composto por diversos códigos;