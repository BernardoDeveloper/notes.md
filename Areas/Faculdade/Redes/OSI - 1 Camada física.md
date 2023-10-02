Notes:
- [[Camada OSI]]

Source: Glauco - UNIP
Project: #project/faculdade 
Areas: #areas/network 
Related: [[Camada OSI]]

---

# Conteúdo

Topologia:
- **física:** Como os dispositivos estão conectados
- **lógica:** Como os dados se transferem

### Topologia física:

- barramento: um cabo, as máquinas se conectam a ele. Um terminador fica na ponta, o dado bate em um ponta e volta. Um cabo em linha reta, adiciono um a rede por um T.
- estrela: conectado a um equipamento central (hub (repetidor)/switch o eqp. central)
- anel: uma máquina liga na outra. Somente quem tem `token` transmite.

### Topologia lógica:

Lógicamente pode funcionar como um anel, mas pode estar físicamente como uma estrela. Somente tenho uma porta de rede.
Frequência diferente, vários dados.
Fibra - por cores diferentes

## OSI e TCP/IP

OSI foi criado pela ISO → para padrão
Camada 5 - sessões (várias abas do navegador)
Cada camada trata os dados de uma maneira diferente, forma de tratar os dados → o que vai em cada pacote, em cada dado a montagem deles → head e etc.
