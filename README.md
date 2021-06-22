# Data-Management-Systems-Benchmark-SSB-Analysis
Data Management Systems Benchmark SSD Analysis

Este primeiro projeto tem como principal objetivo a aquisição de competências no domínio de estudos de benchmarking em base de dados. Com isso em mente, foi analisado a performance do motor de base de dados Postgres.
## Processo Experimental
Todos os passos desde projeto, excepto a geração dos dados no SSB, foram realizados em duas máquinas distintas e com configurações de hardware ligeiramente diferentes. Com isso em mente, o trabalho apresentado neste documento visa não só uma análise do comportamento do motor de base de dados Postgres, mas tem também como objetivo comparar o seu comportamento em máquinas diferentes.
O primeiro passou consistiu em gerar aproximadamente 10GB de dados (para um scale-factor de 15 o SSB não gerou 15GB). Tal como referido anteriormente, este foi o único passo que foi realizado apenas numa máquina, uma vez que o que pretendíamos avaliar era a performance do Postgres e não do SSB.
Todos os passos que se seguiram, foram realizados em duas máquinas distintas. De modo a ser possível assumir uma distribuição normal da amostra dos dados recolhidos, foram realizadas 35 repetições de cada operação de inserção (load), pesquisa (search) e criação de chaves primárias (PK) e estrangeiras (FK).
Depois de realizadas todas as repetições das operações, os dados recolhidos foram processados, analisados e apresentados no presente documento.
Com base no objetivo geral do projeto e dos requisitos descritos no enunciado a performance será medida e avaliada com base no tempo de execução das pesquisas. Neste caso, os resultados com um tempo de execução mais baixos significam que são mais rápidos e por sua vez mais eficientes. Em adição, no processo de carregamento dos dados, serão também avaliados o número de linhas e os megabytes carregados por segundos.
