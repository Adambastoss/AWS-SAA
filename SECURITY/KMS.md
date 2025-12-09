O AWS KMS oferece **chaves multirregionais (MRKs)**. Você pode criar uma chave primária em uma região e ter réplicas dessa mesma chave em outras regiões. Todas as réplicas compartilham o **mesmo ID de chave e material de chave**, permitindo que você as use de forma intercambiável. Isso atende perfeitamente ao requisito de usar "a mesma chave" em duas regiões.

- É um **serviço totalmente gerenciado** e altamente disponível.
    
- Fornece **armazenamento seguro de chaves** (HSMs).
    
- Oferece **integração nativa** com a maioria dos serviços da AWS (S3, EBS, RDS, etc.).
    
- Permite **controle de acesso granular** via políticas do KMS e IAM.
    
- Suporta **rotação automática de chaves** para chaves gerenciadas pela AWS.

Projetado especificamente para criar e controlar chaves de criptografia usadas para criptografar dados.

