
### **Amazon RDS Proxy**

O **Amazon RDS Proxy** é um **proxy de banco de dados totalmente gerenciado** pela AWS que fica **entre a aplicação e o banco de dados RDS/Aurora**:

Aplicação
   ↓
RDS Proxy
   ↓
RDS / Aurora

### Funcionamento técnico

1. A aplicação **não conecta diretamente ao banco**
    
2. Ela conecta ao **endpoint do RDS Proxy**
    
3. O Proxy:
    
    - Mantém um **pool de conexões persistentes**
        
    - Reutiliza conexões já abertas
        
    - Controla quantas conexões chegam ao banco
        
4. O banco de dados recebe:
    
    - Menos conexões
        
    - Conexões mais estáveis
        
    - Menos picos

O RDS Proxy serve para:

1. **Reduzir o número de conexões abertas no banco**
    
2. **Evitar esgotamento de conexões**
    
3. **Aumentar a resiliência durante failover**
    
4. **Melhorar a performance de aplicações altamente concorrentes**
    
5. **Centralizar e proteger credenciais**

### ❌ Sem RDS Proxy

Exemplo com AWS Lambda:

- Cada execução Lambda:
    
    - Abre uma nova conexão
        
- 1.000 execuções simultâneas
    
- 1.000 conexões abertas no banco
    
- Banco cai ou fica instável