Controle de recursos para usuários -> gerenciar permisões de recursos da AWS
Podemos dar os acessos aos usuários atráves de *permissões diretas* a eles mesmo ou por *grupos*
Um **usuário** pode ter muitos **grupos** | 1 para N

+ Os recursos AWS podem ser acessados por **CLI, SDK** ou **Dashboard**

As permisões são criadas por uma **policy** que é um documento `.json` com as permissões que um grupo IAM ou usuário tem acesso.

**IAM Role** - uma identidade (temporária) que define o que tem acesso e o que não tem. Quando associada a um usuário ele deixa de ter suas permissões e exerce a da role.

EC2 vai acessar um S3 - EC2 comunica com um *Role* que tem as permissões de um *policy* e com base nessas permissões o *Role temporário* fornece o acesso aos dados do S3

**ex.** um *IAM User* tem um acesso restrito (fornecido por uma `policy`) ao bucket que definirá o que ele terá permissão. \* Mas quando esse usuário precisar realizar operações de um *admin* ele pode assumir um **role** com as devidas permissões e acessar o S3 como admin, depois sua *policy* padrão reotrna a ele.

**Acess advisor** - quais serviços X um *IAM User* tem acesso

---

[ADM](https://837505506561.signin.aws.amazon.com/console):
User: BernasDevopis
Password: i}0T5(iT
