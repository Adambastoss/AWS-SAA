
Uma empresa possui uma tarefa de extração, transformação e carregamento (ETL) do AWS Glue executada todos os dias no mesmo horário. A tarefa processa dados XML armazenados em um bucket do **Amazon S3**. Novos dados são adicionados ao bucket do S3 todos os dias. Um arquiteto de soluções observa que o AWS Glue processa todos os dados durante cada execução.

O que o arquiteto de soluções deve fazer para **evitar que o AWS Glue reprocesse dados antigos**?

- **Marcadores de Trabalho (Job Bookmarks):** ✅ Este é o **recurso específico do AWS Glue** projetado para resolver exatamente esse problema.
    
- **Como Funciona:** ✅ Quando habilitado, o Glue **rastreia os dados que já foram processados** em execuções anteriores do mesmo trabalho. Na próxima execução, ele **processa automaticamente apenas os dados novos ou alterados** desde a última execução bem-sucedida.