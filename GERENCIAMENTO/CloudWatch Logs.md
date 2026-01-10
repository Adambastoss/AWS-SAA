 Existe uma integração nativa e direta entre **CloudWatch Logs** e **OpenSearch Service**
 
 **Integração Nativa e Gerenciada:** ✅ O CloudWatch Logs possui um recurso chamado **"Assinaturas de Fluxo de Dados (Subscription Filters)"**. Você pode configurar uma assinatura que **transmite os logs em tempo real diretamente para o Amazon OpenSearch Service**.

### **Amazon CloudWatch Custom Metrics**

O **Amazon CloudWatch Custom Metrics** permite enviar ==métricas== personalizadas (como tempo de resposta de uma API) diretamente ao CloudWatch usando a API PutMetricData. Em seguida, é possível criar alarmes no CloudWatch com base nessas métricas, acionando notificações ou ações automáticas quando os limites forem excedidos.