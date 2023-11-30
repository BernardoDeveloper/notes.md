
## Geração do Código
Primeiro a todos os disipositivos que tivermos para arrumar, teremos que gerar um código aleatório e único. Esse código deve ser gerado e inserido no banco de dados contendo as seguintes informações:

| código_dispositvo (único) | nome_do_cliente (único) | cpf_cliente (único) | numero_para_contato |
| --- | --- | --- | --- |
| iphone7plus-preto-bernardo-48426208894 | bernardo gualberto silva | 48426208894 | 11969235721 |

Relacionando a tabela dos dados do cliente com a de dispositvos contendo as informações do dispositivo X, cada usuário pode ter N dispositivos;

| código_dispositivo | marca | modelo | cor | descricao_manutencao | orcamento_valor | orcamento_aprovado | status_id |
| --- | --- | --- | --- | --- | --- | --- | --- |
| iphone7plus-preto-bernardo-48426208894 | apple | iphone7plus | preto | troca da tela | 850.00 | true | 0 |

Tabela de status:

| status_id | descricao |
| --- | --- |
| 0 | não iniciado |
| 1 | esperando aprovar o orçamento |
| 2 | realizando a manutenção |
| 3 | finalizado |

### Forma de registrar um cliente
**Adm:**
Ao acessar a página `/a_definir` poderá definir as informações do cliente como nome, cpf e número para contato. Depois do usuário registrado irá informar os dados do celular como marca, modelo, cor, descrição sobre a manutenção (ex. realizar a troca da bateria), iniciará o orçamento como zero, iniciará com o orçamento aprovado como falso e o status como 0 de não iniciado.

**Usuário:**
Acessando a página `/a_definir` o usuário poderá informar qual o código do celular e o seu cpf para provar que o dispositivo é dele, e será informado o valor do orçamento se estiver como falso, o usuário poderá aprovar (mostrar mensagem informando que não poderá reverter o valor), e a baixo terá as informações do status de como está a manutenção do dispositivo e qual técnico está realizando a manutenção do dispositvo.

**Adm:**
Acessando a página `/a_definir` o administrador poderá informar o código do dispositivo e definir qual o status e o andamento do concerto do dispositivo X.

**Acompanhamento de vídeo:** valor adicional para poder ter acesso a acompanhar a manutenção ao vivo.