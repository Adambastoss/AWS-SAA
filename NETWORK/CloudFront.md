
### **Criptografia em Nível de Campo**

**Field-Level Encryption** permite criptografar **dados específicos (campos)** no momento em que uma visualização HTTPS os envia para o CloudFront, de modo que somente determinados servidores de aplicativos ou serviços na origem possam descriptografá-los.


1. Você configura um **perfil de criptografia** no CloudFront que especifica os campos a serem criptografados (por exemplo, `"credit-card-number"`) e a **chave pública** do destinatário autorizado.
    
2. Quando um usuário envia um formulário, o CloudFront **criptografa os campos especificados** com a chave pública **antes de encaminhar a solicitação para a origem**.
    
3. Apenas o serviço de origem que possui a **chave privada correspondente** pode descriptografar esses campos.

