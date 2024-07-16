Related: [[ofcdesk]]

---

**Procore Integration (Bernardo):** Entrar no Procore
⚠️ IMPORTANTE ⚠️ Criar um private APP dentro do Procore, o Procore vai rodar e irá enviar os dados para *Systems Hub*

Dentro do Procore terá duas principais entidades o Submitals & RFI Workflows
**Task:** criar uma tabela informando o que é possível e o que não é possível, criar uma tabela com os dados sobre o que podemos ter de dados e o que não teremos

Procore ERP - enviar os dados
**Task:** gerar um token dentro do Procore e enviar para algum endpoint público

System Hub (output é o ACC) - receber os dados -> ele conecta no ACC

**Task:** dentro do Procore, irá criar um token e esse token será gerado via user input (usuário clicando em algum lugar) e toda vez que eu for comunicar com o siHub eu utilizo esse token

#### Fluxo do sistema
O app do Procore terá um trigger no na entidade do RFI e do Submitals e toda vez que for disparado ele deve fazer o cadastro dentro do siHub
![[2 - Areas/Trabalho - OFCDesk/Ponds/Fluxo do sistema.canvas|Fluxo do sistema]]

#### Documentações
1. ACC Autodesk Countruction Cloud API's
2. siHub Swagger API
