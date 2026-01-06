Serviço de sistema de arquivos de rede ==totalmente gerenciado==. Ele é projetado para ser **altamente disponível e durável** por padrão, armazenando dados de forma **redundante** em várias Zonas de Disponibilidade dentro de uma região.

**Acesso Compartilhado:** O EFS pode ser montado simultaneamente em **múltiplas instâncias EC2** em várias Zonas de Disponibilidade. Isso significa que todas as instâncias podem acessar o mesmo catálogo centralizado.

O Amazon EFS é um serviço de sistema de arquivos compatível com NFS, ==projetado para Linux==, **não para Windows**. *Instâncias Windows não suportam nativamente NFS* sem configurações adicionais complexas e não é a solução recomendada para Windows.