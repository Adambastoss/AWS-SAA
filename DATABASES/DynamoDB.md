### ==Mecanismo de **backup nativo** e **gerenciado** do DynamoDB==

- **Recuperação Pontual (PITR):** ✅ Quando habilitado para uma tabela do DynamoDB, o PITR cria **backups contínuos** dos dados, permitindo que você restaure para qualquer ponto no tempo dentro dos últimos 35 dias.

- **Atende ao RPO de 15 minutos:** ✅ Com o PITR habilitado, você pode restaurar para um ponto específico com **precisão de segundos**. Isso significa que, em caso de corrupção de dados, você perderá no máximo os dados escritos nos segundos/minutos anteriores ao incidente, facilmente atendendo a um RPO de 15 minutos.

### **Amazon DynamoDB Accelerator (DAX)**

A solução que **melhora diretamente o desempenho de leitura do DynamoDB sem reconfigurar o aplicativo** é o **Amazon DynamoDB Accelerator (DAX)**.

- **DAX** é um **cache em memância totalmente gerenciado e compatível com a API do DynamoDB**. Ele é projetado especificamente para acelerar as leituras do DynamoDB.
    
- A principal vantagem é a **compatibilidade total da API**: você **não precisa modificar o código do aplicativo**. Basta apontar a aplicação para o **endpoint do DAX** em vez do endpoint do DynamoDB. O DAX atua como um proxy de cache; se os dados estiverem no cache, ele os retorna com latência de microssegundos; se não, busca no DynamoDB e armazena em cache.
    
- **Reduz sobrecarga operacional** por ser um serviço totalmente gerenciado.