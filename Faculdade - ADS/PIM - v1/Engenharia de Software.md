> Ideia do projeto: Criação de um sistema para o gerenciamento de museu que contêm diversos temas.

### Requisitos:
1- Mostrar aos usuários quais são os principais temas, com base nas pesquisas realizadas nos respectivos temas. Definindo como os temas iniciais: 100 anos da semana da arte moderna, 150 anos de Santos Dumont e Jogos Olímpicos de París de 2024.

2- A aplicação consiste em um terminal separado em duas parte, uma das com o conteúdo rankeado diponibilizando os temas para serem visualizados e a outra com os dados do determinado tema.

3- O sistema deverá integrar diversos terminais, para disponibilizar tal funcionalidade teremos um arquivo disponível na rede que contenha os dados de cada tema (titulo, descrição, pesquisa e etc) e cada terminal terá acesso ao mesmo arquivo sendo possível disponibilizar os mesmo em cada um dos dispositivos.

### Fluxo grama do sistema:
Teremos o nosso sistema divido em duas partes uma delas irá conter duas colunas, sendo a da esquerda mostrando os temas listados de forma rakeada a partir da pesquisa realizada para cada tema, e a coluna da direita mostrando o tema selecionado e disponiblizando um link para realizar uma pesquisa sobre o respectivo tema, tal pesquisa estará localizada em uma outra página da aplicação contendo as informações e perguntas sobre o tema em questão, após a finalização da mesma, será redirecionada para a tela incial mostrando os temas e seus respectivos conteúdos.

> A fazer: sistema de **pagamento**

![[fluxo_grama.png]]

---

### Estrutura do sistema:
Nosso software será estruturado, com o design pattern *Singleton*, que consiste na criação de uma classe de base instanciando todos os outros objetos. Seguiremos um padrão para antes do envio a branch principal do Github realizar os testes unitários, para evitar erros na aplicação.

### Tecnologias utlizadas:
+ Linguagem de programação: C;
+ Bibliotecas: -;
+ Protocolo de comunicação: HTTP;