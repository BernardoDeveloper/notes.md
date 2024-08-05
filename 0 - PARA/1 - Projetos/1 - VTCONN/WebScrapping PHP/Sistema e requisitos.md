Related: [[WebScrapping Wagner PHP]]

---

**Qual o problema a ser resolvido?**
Capturar informações para que possam ser utilizadas no BI

**Como será resolvidor?**
Extrair os dados da API do Bling e as informações devem ser passadas para um arquivo `.csv`

**Problema encontrado:** a API tem um token de acesso que é gerado de tempos em tempos, necessário criar um *job* com php para ficar realizando a requisição na API e não perder o acesso

O que preciso para desenvolver *token* de acesso da API do **bling**, e depois do processo de [authentication na API](https://developer.bling.com.br/autenticacao) teremos acesso para realizar as requisições

### Requisitos Funcionais (RF)
Funções e informações que o software deve possuir, ou seja como ele deve reagir

1. Buscar dados na API do Bling
	1. Parte técnica: utilizar o [curl](https://stackoverflow.com/questions/9802788/call-a-rest-api-in-php)
2. Exportar dados para *planilhas excel*
	1. Parte técnica: de array para `.xls` [artigo de exemplo](https://stackoverflow.com/questions/10424847/export-an-array-of-arrays-to-excel-in-php)

### Requisitos Não funcionais (RNF)
É necessário para a qualidade do produto, relacionado a qualidade específicas e/ou restrições do sistema

1. Não desconectar o token de acesso da API do Bling
2. Interface WEB para baixar as planilhas e fazer a requisição dos dados

> O ponto mais crucial será a questão de authentication

**Prazo definido:** 2 semanas