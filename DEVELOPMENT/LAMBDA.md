Por padrão, uma função Lambda é executada em uma **rede gerenciada pela AWS** e **não tem acesso direto a recursos em uma VPC** (como uma instância EC2) ou, por extensão, a redes locais conectadas à VPC.

Para que uma função Lambda acesse recursos em uma **sub-rede privada** (seja na VPC ou, através da VPC, em um data center local conectado via Direct Connect/VPN), você deve **configurar a função Lambda para ser executada dentro da VPC**.

---------------
