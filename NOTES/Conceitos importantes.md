## CloudWatch
#### Situação:
O gerente de produto da empresa precisa acessar esse painel (do **CloudWatch**) periodicamente. O gerente de produto não possui uma conta na AWS.
#### Solução:
Compartilhe o painel do console do CloudWatch. Insira o endereço de e-mail do gerente de produto e conclua as etapas de compartilhamento. Forneça um link compartilhável do painel com o gerente de produto.

O Amazon CloudWatch possui um recurso de **compartilhamento de painel** integrado.

Quando você compartilha um painel do CloudWatch, o destinatário **não precisa de uma conta da AWS** para visualizá-lo. Eles simplesmente seguem o link no navegador.

--------------------------------------------------------------------------
## Global Accelerator

Ele usa o **pool de IPs estáticos da AWS Edge Location** para direcionar o tráfego do usuário para endpoints de aplicação saudáveis em uma ou várias regiões da AWS.

Funciona na **camada de rede** (Camada 3) e pode otimizar o roteamento para **qualquer protocolo**, incluindo UDP, que é crucial para o serviço de ==VoIP==.
