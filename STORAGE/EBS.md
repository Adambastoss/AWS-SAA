### **EBS Multi-Attach:**

O EBS Multi-Attach permite que um _mesmo_ volume EBS seja anexado a várias instâncias EC2 **na mesma Zona de Disponibilidade**. Anexar os volumes de _produção_ diretamente ao ambiente de teste significa que **qualquer modificação no teste afetaria diretamente os dados de produção**

### **Fast Snapshot Restore – FSR**

Este é o elemento crucial que minimiza o tempo. Ao ativar o FSR em um snapshot do EBS, você pré-provisiona um armazenamento de alto desempenho para esse snapshot em uma Zona de Disponibilidade específica.

Quando você restaura um snapshot com FSR ativado em um novo volume EBS, esse volume é **instantaneamente criado com todo o seu desempenho máximo**, sem a latência inicial de "aquecimento" associada à restauração padrão de snapshots.