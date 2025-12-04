### ==Mecanismo de **backup nativo** e **gerenciado** do DynamoDB==

- **Recuperação Pontual (PITR):** ✅ Quando habilitado para uma tabela do DynamoDB, o PITR cria **backups contínuos** dos dados, permitindo que você restaure para qualquer ponto no tempo dentro dos últimos 35 dias.

- **Atende ao RPO de 15 minutos:** ✅ Com o PITR habilitado, você pode restaurar para um ponto específico com **precisão de segundos**. Isso significa que, em caso de corrupção de dados, você perderá no máximo os dados escritos nos segundos/minutos anteriores ao incidente, facilmente atendendo a um RPO de 15 minutos.
