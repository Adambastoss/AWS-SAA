
### WAF e CloudFront

Uma empresa executa seu site em instâncias do Amazon **EC2** por trás de um **Application Load Balancer** configurado como origem para uma distribuição do Amazon **CloudFront**. A empresa quer se proteger contra **scripts** entre sites e ataques de **injeção** de SQL.

Qual abordagem um arquiteto de soluções deve recomendar para atender a esses requisitos?

**Configure o AWS WAF na distribuição CloudFront. Use condições e regras que bloqueiem scripts entre sites e ataques de injeção SQL.

--------------------------------------------------------------------------


### VPN

Quais componentes são necessários para construir uma conexão VPN site a site com a AWS?

Um **Gateway de cliente** 
É necessário um gateway de cliente para que a conexão VPN seja estabelecida. Um dispositivo de gateway do cliente é configurado no data center do cliente.

Um **Gateway privado virtual**
Um gateway privado virtual é conectado a uma VPC para criar uma conexão VPN site a site com a AWS. Você pode aceitar tráfego de rede criptografado privado de um data center local para sua VPC sem a necessidade de atravessar a internet pública aberta.