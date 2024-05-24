Source: Bernardo
Related: [[1 - Aprendizado, Treinamentos]]

---

Foco do financeiro ele trata de saldos bancários, foco é gerenciar as contas a pagar e receber -> deixando o saldo gerenciavél

Precisamos de um *banco* configurado pois ele será responsável por dar baixa no seu dinheiro a receber e ao pagar.

**Contas a receber:** relacionado a notas fiscais de saída -> títulos das vendas que foram realizadas;
**Contas a pagar:** tudo o que você comprou;
**Natureza:** controle a todas as finanças a pagar e a receber -> classifica também os títulos a pagar ou a receber;

**TES:** é uma *automatização* ela vai permitir o cadastro automático de entrada e saída no ERP. Ele vai definir se uma determinada operação é de venda ou de compra.

`Código:` 000-500 operação de **entrada** de valores | 501-999 operação de **saída** -> isso é padrão no Protheus. Também ela que define se a operação vai movimentar o estoque, financeiro, gera duplicada ...  
Caso eu tenha uma operação de compra vou utilizar uma TES com o valor menor que 500, uma operação de venda maior que 500

## Fluxo sistema ERP
Preciso de um produto (seus dados, preciso ter ele comprado de um fornecedor e estocado), preciso de um cliente (quem vai comprar o produto, emitir nota fiscal, remover do estoque o que foi comprado), preciso de um banco para fazer todas as transações do meu negócio.

Banco
![[Pasted image 20240110094657.png]]

Fornecedor
![[Pasted image 20240110094943.png]]

Armazem para guardar o produto
![[Pasted image 20240110095317.png]]

Produto para você comprar do fornecedor e também vender
![[Pasted image 20240110095602.png]]

Preciso emitir um pedido de compras para o meu fornecedor pedindo para que ele me envie X produto.
Condição de pagamento
![[Pasted image 20240110100149.png]]
Pedido de compra do produto e em qual estoque será armazenado
![[Pasted image 20240110100346.png]]
Preciso de um *aprovador* para liberar o meu pedido
![[Pasted image 20240110100452.png]]
Pedido já ficou como liberado, quando temos uma **alçada de compras** configurada ou seja os usuário que são compradores, solicitantes e aprovadores.
Depois transformo o pedido em uma *nota fiscal* de entrada, precisamos definir uma TES de entrada.
![[Pasted image 20240110101255.png]]
Com isso o estoque é alimentado com o produto, agora que dei entrada posso dar a saída nesse produto.
![[Pasted image 20240110133040.png]]

OBS: fiquei travado por um tempo, pois eu realizava um pedido de compra corretamente, mas não aparecia o mesmo no meu estoque, pois o TES que eu tinha configurado não estava com a atualização de estoque configurado.

> fifo e lifo: first input e first output, last input e last output

Com o produto em estoque podemos dar um saída a ele via modulo de faturamento, podendo criar os PV (Pedidos de venda), para isso precisamos de um cliente.
![[Pasted image 20240110130141.png]]

Para vender um produto, precisamos de vendedores
![[Pasted image 20240110130433.png]]

Depois liberamos o crédito dele
![[Pasted image 20240110141549.png]]
Assim gerando uma nota fiscal

