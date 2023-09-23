> Ideia do projeto: Criação de um sistema para o gerenciamento de museu que contêm diversos temas.

### Requisitos:
1- Mostrar aos usuários quais são os principais temas, com base nas pesquisas realizadas nos respectivos temas. Definindo como os temas iniciais: 100 anos da semana da arte moderna, 150 anos de Santos Dumont e Jogos Olímpicos de París de 2024.

2- A aplicação consiste em um terminal separado em duas parte, uma das com o conteúdo rankeado diponibilizando os temas para serem visualizados e a outra com os dados do determinado tema.

3- O sistema deverá integrar diversos terminais, para disponibilizar tal funcionalidade teremos um arquivo disponível na rede que contenha os dados de cada tema (titulo, descrição, pesquisa e etc) e cada terminal terá acesso ao mesmo arquivo sendo possível disponibilizar os mesmo em cada um dos dispositivos.

### Forma de funcionamento:
Teremos o nosso sistema divido em duas partes uma delas irá conter duas colunas, sendo a da esquerda mostrando os temas listados de forma rakeada a partir da pesquisa realizada para cada tema, e a coluna da direita mostrando o tema selecionado e disponiblizando um link para realizar uma pesquisa sobre o respectivo tema, tal pesquisa estará localizada em uma outra página da aplicação contendo as informações e perguntas sobre o tema em questão, após a finalização da mesma, será redirecionada para a tela incial mostrando os temas e seus respectivos conteúdos.

> A fazer: sistema de **pagamento**

![[fluxo_grama.png]]

---
### Tecnologias utlizadas:
+ Linguagem de programação: C;
+ Bibliotecas: null;
+ Protocolo de comunicação: HTTP;

---

### Tarefas:
- [ ] Levantamento detalhado dos requisitos - Hudson;
- [ ] Planejar o sistema, a forma que os terminais vão se relacionar entre si - Todo mundo;
- [ ] Separar as tarefas para cada requisito (para construir um RF temos que definir quais são as tarefas para obter o resultado) - Matheus Corsa;
- [ ] Arquitetura do sistema (modelo ágil, cascata, espiral, etc...) - Matheus Corsa & Hudson;
- [ ] Finalizar o fluxo grama do sistema - Bernardo;
- [ ] Preparação para codificar, configurar como a gente vai desenvolver, criar a arquitetura e organização das pastas com os códigos - Matheus Celta;
- [ ] Codificação - Todo mundo (pelo menos cada um desenvolver uma funcionalidade);
- [ ] Testes - Inicialmente: a cada funcionalidade que for desenvolvida, criar um teste para ela | Futuramente: caso sobre tempo realizar os testes por código - Matheus Celta & Bernardo;