Source: Bittencourt
Related: [[Sistemas Orientado a objetos]]

---

**Legenda:**
SW: Software
### Projeto de desenvolvimento de software
- Estpecificação de SW: requisitos, regras de execução, diagramas e etc...
- Projeto de implementação de SW: Transformando os requisitos em sistema de SW
- Validação de SW: Fase em que validamos se o sistema está conforme desejamos
- Evolução do SW: Montamos estratégias para escalar e mantar o SW

**Exemplo:** Manter o usuário
Precisamos seguir várias etapas dentre elas, os requisitos identificados na especificação do projeto:
1. Validação
2. Inserir
3. Alterar
4. Listar
5. Buscar
6. Excluir
7. Relatório
8. Exportar para `excel`

Para documentar nos montamos um diagrama com cada um dos requisitos. Um caso de uso por exemplo *validar* ele **extende** do manter usuário.

> Matriz de ratreio: criar uma matriz de rastreio, posso definir uma tabela onde por exemplo o requisito 1 está sendo resolvido pelo *caso de uso 1*.

| Requisito | UC001 | UC002 |
| --------- | ----- | ----- |
| Req. 1    | X     | -     |
| Req. 2    | X     | X     |

Precisamos definir uma descrição para um *caso de uso* definindo nome, atores, evento (principais e alternativos) e regra de negócio. Essa descrição informa o que o usuário acessa, o que irá retornar uma "história".
No planejamento eu **defino** como fazer
Na programação e **ensino** como usar
E para as especificações que iremos fazer definimos qual metodologia iremos utilizar para implementar o que foi pedido como modelo cascata, incremental, prototipagem, ...

**Objeto:** um contexto em geral como por exemplo o contexto de vendas, compras, ...

![[Diagramação de um sistema.canvas|Diagramação de um sistema]]

Ideia de prototipar e montar o que precisa para auxiliar com o levantamento de requisitos

Métricas de software: ponto por função (regra de funcionalidade - complexidade alta, média, baixa)