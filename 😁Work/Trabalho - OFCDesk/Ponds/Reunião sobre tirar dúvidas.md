Related: [[ofcdesk]]

---

Procore: ele é um ERP e iremos desenvolver um custom app dentro dele, estilo um plugin
SiHub (System Hub): uma camada de abstração para comunicar com o AutoDesk
ACC: endpoints da AutoDesk

A Pond não vai utilizar a aplicação em si, mas os clientes da Pond que irão utilizar o Procore.
#### TODO:
- [ ] Procore: criar um custom App.
- [ ] O custom app precisar listar as entidades de um projeto:
1. lista de Submitals
2. lista de RFIs
3. triggers: uma vez que teve a conexão, basicamente eu vou analisar o RFIs e se alterar ele deve mandar para um endpoint a mesma coisa para o submitals
- [ ] O SiHub irá comunicar com o Procore e irá enviar um dado para o Procore ou para o custom APP

- [ ] Estudar na documentação como faz para criar um custom App.
- [ ] No procore vou instalar o app que eu vou desenvolver.
- [ ] O deshboard irá analisar os RFIs e Submitals.

