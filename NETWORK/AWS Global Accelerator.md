O **AWS Global Accelerator** é um serviço gerenciado da AWS que melhora a **performance, disponibilidade e segurança** de aplicações que atendem usuários ao redor do mundo. Ele atua na **camada de rede (camada 3/4)**, criando um ponto de entrada global fixo para o tráfego dos usuários através de **endereços IP estáticos anycast** e usando a **rede global da AWS** para otimizar rotas.

Ele é ideal para aplicações que precisam de:

| Objetivo                                    | Exemplo de uso                                                           |
| ------------------------------------------- | ------------------------------------------------------------------------ |
| 📈 Reduzir latência global                  | APIs, aplicações globalmente distribuídas, SaaS.                         |
| ⛑ Alta disponibilidade entre regiões        | Failover rápido entre múltiplas regiões AWS.                             |
| 🎮 Baixa latência e estabilidade            | Jogos multiplayer, aplicações de VoIP, streaming em tempo real.          |
| 🔐 Simplificar configuração de firewall     | Com IP estáticos anycast, evita mudanças constantes no DNS ou bloqueios. |
| 💼 Cenários de recuperação de desastre (DR) | Transição quase instantânea para outra região saudável.                  |
✅ **IP estático anycast global:** Um ponto de entrada fixo, sem depender de DNS, simplifica firewalls e clientes.

🧭 **Roteamento inteligente por proximidade e integridade:** Direciona o cliente ao endpoint ideal e mais próximo.

🛡️ **Proteção DDoS integrada com AWS Shield Standard** (camada básica).

Funciona com load balancers, instâncias EC2, Elastic IPs, e até com IPs personalizados (BYOIP).
