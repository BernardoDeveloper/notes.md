Source: Harvard - Computer Science
Project: #project/studies 
Areas: #areas/cs50
Related: [[Life]]

---

[SQL Advanced course](https://youtube.com/playlist?list=PL1XF9qjV8kH12PTd1WfsKeUQU6e83ldfc&si=EXnSAb2FtMDwXfay)
[Training teste](https://leetcode.com/tag/database/)
[Hackerank](https://www.hackerrank.com/domains/sql)

Todas, ou a grande maioria das aplicações tem relações com dados que podem ser gerenciados, para isso utilizamos o SQL um linguagem para manipulação de dados ler, escrever, realizar edição em um geral. Os banco de dados são como arquivos `.csv` eles se organizam por tabelas, colunas e linhas.

**With:** No Visual Basic é muito utilizada para acessar os métodos ou propriedades de um objeto.

No geral sempre precisamos inicializar o local que vamos realizar a edição, por exemplo abrir um arquivo ou uma conexão com o banco de dados.

> $inicializaçãoDoQueEditar (file, dbConnection) > ediçãoDosValoresDesejados > resultadoEsperado$

**Dictionary (Array):** Um conjunto de chave valor, onde posso selecionar a chave que eu quero o valor respectivo da mesma

## Banco de dados relacional - SQL
Estruturas para armazenar muitos dados de forma que se relacionam, NoSQL é o oposto sendo para aramzenar os dados sem terem um relação direta entre si.
SQL faz basicamente **CRUD** (Criar, Ler, Atualizar e Deletar)

**COUNT:** Quantidade de linhas de um retorno, por exemplo `COUNT(<tabela_para_pesquisar_quantidade>)`
**DISTINCT:** Não retorna valores repetidos, por exemplo na coluna X tenho 23 valores *A* e 25 valores *B* então me retorna somente: na coluna X tenho A e B - `DISTINCT(X)`

![[Pasted image 20231104075310.png]]

**WHERE:** Filtrar valores.
**LIKE:** Retornar algo se tenha X alguma coisa
**ORDER BY:** Forma de ordernar os dados
**LIMIT:** Limita a quantidade de linhas que irá retornar
**GROUP BY:** Juntar os valores de uma coluna com a outra, por exemplo agruapr nome, e o count de nome. `GROUP BY column_name`
**FILTER:** AVG, LOWER, MAX, MIN, UPPER, LIKE

