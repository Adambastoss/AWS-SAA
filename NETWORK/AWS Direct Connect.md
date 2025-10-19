O **AWS Direct Connect** estabelece uma **conexão de rede privada dedicada** entre seu datacenter local e a AWS. Isso **ignora completamente a internet pública** para o tráfego de backup.

-------------------------------------------------------------------------
### ==**Application Load Balancer**==

Possui uma funcionalidade integrada para **redirecionamento**. 
Você pode criar um **ouvinte (listener)** na porta 80 (HTTP) e configurá-lo com uma regra de ação do tipo **"Redirecionar para"**, especificando a porta 443 (HTTPS) e o protocolo HTTPS.

Quando um usuário tenta acessar o site via `http://`, o ALB automaticamente responde com um redirecionamento HTTP 301 ou 302 para a URL `https://` equivalente, forçando o uso de uma conexão segura. Isso é a maneira padrão e recomendada de implementar o **redirecionamento** HTTP para HTTPS.