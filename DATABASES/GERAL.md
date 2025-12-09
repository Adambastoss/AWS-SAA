A única maneira de habilitar a **criptografia** em uma **instância de banco** de dados do **RDS** que ==atualmente não é criptografada== é:

1. Criar um **snapshot** da instância existente.
    
2. **Copiar** esse snapshot e **habilitar a criptografia** durante o processo de cópia (usando uma chave do AWS KMS).
    
3. **Restaurar** o novo snapshot criptografado para criar uma **nova instância de banco de dados RDS criptografada**.
    
4. Modificar o aplicativo para apontar para o novo endpoint do banco de dados criptografado e, por fim, descomissionar a instância antiga não criptografada.