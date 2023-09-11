+ Cloud computing: cliente -> network -> server `analogia da carta de correio`

Com servidores próprios temos que preocupar com toda a *infraestrutura* como energia, rede, segurança entre outras coisas, logo também com os gastos.
Em *cloud* trabalhamos com recursos computacionais sob demanda ou seja pagamos o que estamos usando, e usamos somente o que precisamos.

On-premises: Você paga pelo seu serviço, pelo seu servidor, pela sua energia
Cloud provider: Outras pessoas cuidam do seu servdior, eles cuidam da energia, da sua infra no geral

**VPS** - uma máquina rodando várias
**Shared Hosting** - vários clientes na mesma máquina
**Cloud Hosting** - várias máquinas físicas com vários clientes

### Termos:
**CSP**: Cloud Service Provider
+ Vários serviços, para oferecer um Cloud hosting

**SaaS** - Software como serviço: produto como serviço não se preocupa com nada somente a aplicação
**PaaS** - Plataforma como serviço: foco em desenvolver, (ex. elastic beans e heroku)
**IaaS** - Infraestrutura como serviço: Blocos de infraestrutura, para processamento, armazenamento e rede. Não se preocupar com o código mas sim onde ele vai ser executado

**Preço:**
+ Compute: compute time
+ Storage: data stored
+ Data transfer: transfer in free

*Data Governance:* condição para estar de acordo com os negócios.
*Region:* cluster (CPD) de data center

#### Região:
Cada zona possui *regiões* que contêm um conjunto de servidores para realizar um load balancer, obtendo maior performance dos servidores.

### Serviços
CPS (Cloud provider service) - para infra estrutura como serviço
+ Compute - EC2
+ Storage - EBS
+ Database - RDS
+ Networking - VPC

---

### Evolução da computação
+ Servidor físico:
	+ Nunca utiliza 100% do servidor
	+ Está pagando por coisa a mais
	+ Você tem que cuidar e gerenciar de toda a infraestura do seu próprio servidor
	+ Fazer melhorias é mais complexo, em realação a valores e espaço pois em algumas ocasiões serem necessários comprar um novo servidor

+ VMs:
	+ Máquinas dentro de máquinas
	+ Você está utilizando uma parte de uma máquina
	+ Pode compartilhar com diversos colaboradores
	+ Está pagando por uma fração do servidor

+ Containers: Tipo uma VM só que menor, pois está pegando somente o que precisa ao invés de virtualizar uma máquina inteira, você virtualiza somente o que precisa

+ Funciontions: Os desenvolvedores empacotam suas aplicações em containers e colocam em um *serveless* e ele gerencia toda a infraestrutura, espaço necessário, energia, rede ...

### Modelo de Implantação
**Public Cloud:** uma sub núcleo que se encontra em um núcleo maior que cada sub núcleo é compartilhado com as aplicações que está utilizando como por exemplo EC2 para fazer o processamento, S3 Bucket para armazenar, IAM para gerenciar seus acessos ...

**Private Cloud:** Seus servidores físicos
**Hybrid:** A junção dos dois, utilizando por exemplo alguns processos em um servidor físico e conectado por meio de uma vpn utilizando serviços de Provedor Cloud

**Região:** Alguns do serviços como o EC2 por exemplo não estão disponíveis em todas as regiões