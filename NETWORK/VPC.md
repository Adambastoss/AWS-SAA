## VPC

Quando você **cria** uma **vpc**, **automaticamente** são **criados**: ``Tabela de rotas``, NACL e o Security Group Padrão.
**Não criará** automaticamente qualquer **subnet**, e também não criará o **Internet Gateway.**
A amazon sempre reserva **5 endereços** IP's na sua subnet.
Você pode ter apenas **1 Internet Gateway** por VPC

--------------------------------------------------------------------------
### ==VPC Gateway Enpoint==

<<<<<<< HEAD
## **ELB (Elastic Load Balancer**
 
É o recurso **publicamente acessível** que recebe o tráfego direto da web.

**Cenário Realista:** Para uma aplicação web crítica sendo lançada publicamente, proteger o balanceador de carga (que é o alvo mais provável) com Shield Advanced é a recomendação padrão para resiliência contra DDoS.

Ao atribuir o **Shield Advanced** ao seu ELB, você está **protegendo** diretamente o **ponto de entrada** da sua aplicação.
=======
Um **VPC Gateway Endpoint** para o **Amazon S3** permite que o tráfego entre o VPC e o S3 **ocorra principalmente pela rede privada da AWS** , **sem necessidade de Internet, NAT Gateway ou IP público** .

>>>>>>> 7a59c3b7cb7acaef3f2d4ac53160455fb8a59c07

