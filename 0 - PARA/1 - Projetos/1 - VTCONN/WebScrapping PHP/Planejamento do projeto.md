Source: Conversar com o Wagner
Related: [[WebScrapping Wagner PHP]]

---

![[Fluxo do projeto.canvas|Fluxo do projeto]]

![[Pasted image 20240330232007.png]]

### Qual o problema que eu preciso resolver?
Preciso pegar os dados que estão no *ERP da bling* e armazenar em um arquivo `.csv`

**Quais dados preciso pegar do ERP e passar para o CSV?**
1. Nome do cliente
2. Descrição do produto
3. Informações do pedido de venda

> *Técnico:* Com esses dados armazenar em um banco local, e com todos os dados populados, gerar um único arquivo `.csv` a cada 5 horas com as informações atualizadas.

**Arquivo de exemplo:**

| cliente_id | cliente_nome | cliente_codigo                  |     |
| ---------- | ------------ | ------------------------------- | --- |
| bernardo   | camisa       | NF: 0000000000<br>Preço: 123,99 |     |

| id          | nome                                                        | codigo                           | preco | tipo | situacao | formato | descricaoCurta | imagemURL |
| ----------- | ----------------------------------------------------------- | -------------------------------- | ----- | ---- | -------- | ------- | -------------- | --------- |
| 16242195825 | Placa Gelo-x Gel Reutilizável 500ml Kit C/ 2 Unid 17x10x3cm | MLKIT_MLB3382471360_177258140086 | 15.9  | P    | A        | S       |                |           |


## Sistema de autenticação
Para acessar qualquer rota da api é necessário gerar um token pelo OAuth, a API tem o sistema de autenticação com OAuth2 é necessário criar um *job (serviço que executa constamente)* que faz uma requisição, pedindo um token para poder acessar a API.
Com o *token* que é gerado libera o acesso para requisitar as rotas com autenticação por *bearer*

