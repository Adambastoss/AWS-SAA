## VPC

Quando você **cria** uma **vpc**, **automaticamente** são **criados**: ``Tabela de rotas``, NACL e o Security Group Padrão.
**Não criará** automaticamente qualquer **subnet**, e também não criará o **Internet Gateway.**
A amazon sempre reserva **5 endereços** IP's na sua subnet.
Você pode ter apenas **1 Internet Gateway** por VPC

--------------------------------------------------------------------------
### ==VPC Gateway Enpoint==

Um **VPC Gateway Endpoint** para o **Amazon S3** permite que o tráfego entre o VPC e o S3 **ocorra principalmente pela rede privada da AWS** , **sem necessidade de Internet, NAT Gateway ou IP público** .


