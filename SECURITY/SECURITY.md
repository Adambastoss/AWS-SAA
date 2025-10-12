A **conta de gerenciamento** possui um **bucket S3** que contém relatórios de projetos.  
A empresa quer ==**limitar o acesso== a esse bucket** apenas aos ==**usuários de contas pertencentes à organização**== no AWS Organizations.
### Adicione à política do bucket S3 a chave global **aws :PrincipalOrgID** referenciando o ID da organização.

- A chave global **`aws:PrincipalOrgID`**permite **restringir o acesso a recursos apenas para contas dentro de uma mesma organização do AWS Organizations** .
    
- Ao adicionar essa condição na **política do bucket S3** , o acesso será concedido automaticamente **apenas a identidades (usuários, funções, contas)** que fazem parte da organização identificada pelo **Org ID** .


#### **AWS Systems Manager Parameter Store**

É um ótimo serviço para armazenar configurações e segredos. No entanto, ele **não suporta rotação automática de segredos** para bancos de dados Amazon RDS/Aurora.

--------------------------------------------------------------------------
#### **AWS Secrets Manager**
Projetado especificamente para **armazenar e recuperar segredos**, como credenciais de banco de dados.

O Secrets Manager pode **rotacionar automaticamente** as credenciais do banco de dados Aurora em um cronograma definido. Isso elimina a tarefa operacional manual de alterar senhas, que é propensa a erros e esforço significativo.

**Minimiza a Sobrecarga Operacional:** Ao automatizar a tarefa mais complexa (a rotação), o Secrets Manager atende perfeitamente ao objetivo principal.

--------------------------------------------------------------------------

