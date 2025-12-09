
O requisito é **manter a utilização da CPU em torno de 40%** para otimizar o desempenho da aplicação. Isso é um cenário clássico para o **Target Tracking Scaling Policy** (Política de ==**Dimensionamento** por **Rastreamento**== de Alvo) do Auto Scaling.

Uma política de **Target Tracking** funciona definindo uma métrica alvo (neste caso, `CPUUtilization` em 40%) e ajustando automaticamente o número de instâncias no grupo para manter essa métrica no valor especificado, independentemente das flutuações de carga.

