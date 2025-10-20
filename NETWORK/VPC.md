## VPC

Quando você **cria** uma **vpc**, **automaticamente** são **criados**: ``Tabela de rotas``, NACL e o Security Group Padrão.
**Não criará** automaticamente qualquer **subnet**, e também não criará o **Internet Gateway.**
A amazon sempre reserva **5 endereços** IP's na sua subnet.
Você pode ter apenas **1 Internet Gateway** por VPC

--------------------------------------------------------------------------

## **ELB (Elastic Load Balancer**
 
É o recurso **publicamente acessível** que recebe o tráfego direto da web.

**Cenário Realista:** Para uma aplicação web crítica sendo lançada publicamente, proteger o balanceador de carga (que é o alvo mais provável) com Shield Advanced é a recomendação padrão para resiliência contra DDoS.

Ao atribuir o **Shield Advanced** ao seu ELB, você está **protegendo** diretamente o **ponto de entrada** da sua aplicação.

