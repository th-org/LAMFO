---
hide:
  - toc
  - title
---

# **Qual a diferença entre ingestão de dados em lote e em streaming? Cite 2 situações em que cada abordagem é melhor que a outra para análises de dados de esporte**

A ingestão de dados em lote (batch processing) envolve a coleta, armazenamento e processamento de grandes volumes de dados acumulados ao longo do tempo. Os dados são processados de forma periódica, geralmente com uma latência maior, o que é ideal para análises históricas e relatórios agregados.
  
→ Conforme o *GeeksforGeeks* destaca, esse modelo é eficiente para grandes quantidades de dados que não exigem respostas em tempo real [1](#REF1).

<br>

Já a ingestão de dados em streaming (stream processing) trata os dados à medida que eles são gerados, em tempo real ou quase real. Isso permite a detecção imediata de eventos e decisões baseadas em dados atualizados.

 → Como explica o *Atlan*, essa abordagem é essencial quando a velocidade de resposta e a atualidade dos dados são críticos [2](#REF2).

### Situações em que cada abordagem é melhor para análises de dados de esporte

**✅ Quando usar processamento em lote**
Análise de desempenho pós-jogo:
 Compilar e processar dados de vários sensores, estatísticas e vídeos para gerar relatórios detalhados sobre o desempenho de jogadores após a partida.
 → Segundo o *Airbyte*, o processamento em lote é ideal para análises complexas que não precisam de respostas imediatas, permitindo uso intensivo de recursos computacionais [3](#REF3).

**Estudos históricos para melhoria de estratégias**
 Agrupar dados de múltiplos jogos ao longo de uma temporada para identificar padrões táticos e tendências de performance.
 → Conforme aponta o *GeeksforGeeks*, o batch é excelente para cenários que exigem análise de grandes volumes de dados consolidados [1](#REF1).

**✅ Quando usar processamento em streaming**
Monitoramento em tempo real durante partidas:
 Utilizar dados em tempo real de sensores vestíveis ou câmeras para identificar riscos de lesão, fadiga ou padrões táticos durante o jogo.
 → Como afirma o artigo da *Restack*, o uso de IA e streaming em esportes permite decisões rápidas com base em dados ao vivo [4](#REF4).

**Engajamento de torcedores em tempo real**
 Processar dados ao vivo (como jogadas, estatísticas e interações sociais) para gerar conteúdos dinâmicos em aplicativos ou transmissões.
 → De acordo com o *Atlan*, streaming é ideal quando há necessidade de reação rápida e entrega contínua de insights [2](#REF2).


<p style="font-size: 14px;"> Autor: <a href=https://github.com/thaleseuflauzino.>Thales Euflauzino, </a>2025</p>

### Referências

> [1]<a id=REF1></a> GeeksforGeeks. Difference between Batch Processing and Stream Processing. Disponível em : [https://www.geeksforgeeks.org/difference-between-batch-processing-and-stream-processing/](https://www.geeksforgeeks.org/difference-between-batch-processing-and-stream-processing/). Acesso em 01 de maio de 2025.
> 
> [2]<a id=REF2></a> Atlan. Batch Processing vs. Stream Processing. Disponível em : [https://atlan.com/batch-processing-vs-stream-processing/](https://atlan.com/batch-processing-vs-stream-processing/). Acesso em 01 de maio de 2025.
> 
> [3]<a id=REF3></a> Airbyte. Batch vs. Stream Processing in Data Engineering. Disponível em : [https://airbyte.com/data-engineering-resources/batch-processing-vs-stream-processing](https://airbyte.com/data-engineering-resources/batch-processing-vs-stream-processing). Acesso em 01 de maio de 2025.
> 
> [4]<a id=REF4></a> Restack. AI in Sports Analytics and Real-Time Data. Disponível em : [https://www.restack.io/p/ai-in-sports-analytics-answer-real-time-data-processing-cat-ai](https://www.restack.io/p/ai-in-sports-analytics-answer-real-time-data-processing-cat-ai). Acesso em 01 de maio de 2025.
