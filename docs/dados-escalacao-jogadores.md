# **Dados na Escalação de Jogadores.**

### I. Introdução :

* **Importância dos Dados:**

A análise de dados vem se tornando uma ferramenta muito importante para a tomada de decisões no esporte, superando limitações da observação tradicional. Assim, é possível identificar padrões ocultos, assim como avaliar desempenho de forma mais objetiva.

* **Objetivo da Apresentação:**

A análise de dados estatísticos e métricas avançadas molda e otimiza as decisões sobre a escalação de jogadores titulares no futebol profissional moderno. Explorando não apenas *quais* dados são usados, mas detalhando os processos, as métricas-chave e os desafios inerentes à utilização de dados para definir quem entra em campo.

* **Observação:**

É importante lembrar que a busca por otimizar a escalação/time titular através de dados não é exclusiva do futebol. É uma tendência consolidada em muitos esportes de alto rendimento. Com objetivo comum: Maximizar a probabilidade de vitória, gerenciar a carga física dos atletas e explorar fraquezas adversárias através de evidências quantitativas.Embora o princípio seja o mesmo, as métricas específicas e os critérios de decisão variam drasticamente conforme as regras, dinâmica e objetivos de cada esporte.Como por exemplo: No basquete, é essencial monitorar o número de mudanças rápidas de direção, já que a dinâmica do jogo exige movimentos intensos em espaços curtos. Já no futebol, onde o campo é maior e os jogadores percorrem distâncias mais longas, a coleta de dados sobre sprints e distância total percorrida é mais relevante.

### II. Tipos de Dados Utilizados para a Decisão de Escalação:

Segundo a Sports Data Campus [[1]](#REF1), são 4 tipos de dados analisados para otimizar a gestão de elenco – desde métricas físicas e técnicas até indicadores táticos e contextuais – são eles: Dados Físicos e de Carga de Trabalho, Dados Técnicos, Dados Táticos e Dados Contextuais e de Desempenho Relativo.

1. **Dados Físicos e de Carga de Trabalho (Monitoramento e Prevenção):**  
    - **Minutos Jogados (Acumulados e Recentes):** Não apenas evitar lesões, mas gerenciar picos de performance. Analisar a distribuição ao longo da temporada e em blocos de jogos.
    - **Dados de GPS e Rastreamento Fisiológico:** Distância percorrida, distância em alta intensidade (High-Speed Running \- HSR), número de sprints, acelerações/desacelerações, carga metabólica.
        - *Como é usado:* Comparar os níveis atuais com os basais do jogador e com as demandas esperadas da partida/posição. Identificar quedas de rendimento físico ou risco iminente.  
    - **Dados de Recuperação:** Questionários subjetivos (percepção de esforço, qualidade do sono), marcadores bioquímicos (quando disponíveis). *Como é usado:* Indicador adicional para decisões de rotação.

Segundo o Journal of Medical and Biosciences Research [[2]](#REF2) Na análise dos dados físicos de um atleta são analisadas métricas como:

2\. **Dados Técnicos (Avaliação de Habilidade e Execução):**

**Métricas Tradicionais Contextualizadas:**

   - **Gols e Assistências:** Continuam importantes, mas analisar por 90 minutos, tipo de gol/assistência (bola parada, jogada construída), e comparar com métricas de expectativa
   - **Passes Completos:** Segmentar por zona do campo (defensiva, meio, terço final), direção (progressivos, laterais, para trás) e tipo (curto, longo, chave).
   - **Dribles Bem-Sucedidos:** Analisar a taxa de sucesso e *onde* no campo ocorrem (se progridem o jogo ou apenas mantêm a posse).

**Métricas Técnicas Avançadas:**

   - **Expected Goals (xG):** Avalia a *qualidade* da finalização com base em fatores históricos (localização, tipo de chute, ângulo, pressão defensiva).
   - **Expected Assists (xA):** Avalia a *qualidade* do passe que leva a uma finalização.
   - **Expected Threat (xT) / Valor de Posse (PV):** Métricas mais complexas que avaliam o valor de qualquer ação (passe, drible, condução) em termos de aumento da probabilidade de gol.
   - **Passes-Chave e Passes para o Terço Final/Área:** Quantificam a criação direta de oportunidades ou a chegada da bola em zonas decisivas.


3\. **Dados Táticos (Adequação ao Modelo de Jogo e ao Adversário):**  

   - **Mapas de Calor (Heatmaps) e Posição Média:** Visualizar onde o jogador atua predominantemente e se isso corresponde ao papel tático esperado. *Como é usado:* Avaliar disciplina posicional, cobertura de espaços.  
   - **Pressão (Pressures) e Sucesso na Pressão:** Quantificar a atividade defensiva sem bola, crucial para times com pressão alta. Avaliar *onde* a pressão ocorre e se resulta em recuperação de posse. *Exemplo:* Um atacante pode ser preferido a outro com mais gols se seus dados de pressão forem muito superiores e o plano de jogo exigir intensidade na primeira linha defensiva.  
   - **Ações Defensivas por Zona:** Desarmes, interceptações, bloqueios, cortes. Analisar não só a quantidade, mas a *eficácia* (taxa de sucesso em desarmes) e a *localização* (defendendo a própria área vs. no campo adversário).  
   - **Duelos Ganhos (Aéreos e no Chão):** Avaliar a capacidade física e de imposição em disputas diretas. Crucial para zagueiros, volantes e atacantes de referência. Comparar a taxa de sucesso.


**4\. Dados Contextuais e de Desempenho Relativo:**

* **Desempenho Contra Adversários Específicos/Tipos de Adversários:** Histórico do jogador contra o próximo oponente ou contra times com estilos semelhantes (bloco baixo, pressão alta).  
  * **Impacto na Equipe (On/Off Metrics):** Como a equipe performa (em termos de xG a favor/contra, gols marcados/sofridos) quando um jogador específico está em campo versus quando está fora. *Cuidado:* Requer amostras grandes e controle de variáveis (qualidade dos substitutos, etc.).  
  * **Índices de Desempenho Compostos:** Plataformas como [WhoScored](https://www.whoscored.com), [SofaScore](https://www.sofascore.com), ou índices proprietários dos clubes que tentam agregar múltiplas métricas em uma única nota. *Como é usado:* Um ponto de partida rápido para comparação, mas a análise detalhada das métricas subjacentes é essencial.

### III. O Processo de Decisão: Da Análise à Escalação


1. **Coleta e Processamento:** Fontes de dados ([Opta](https://optaplayerstats.statsperform.com/en_GB/soccer), [StatsBomb](https://statsbomb.com/), [Wyscout](https://wyscout.hudl.com/app/), dados de tracking internos), plataformas de análise, papel dos analistas de dados/desempenho.  
   
2. **Análise Pré-Jogo:**  
   
      - **Relatórios Individuais:** Perfis detalhados dos jogadores do elenco, comparando métricas chave para a posição, forma recente, carga física.  
      - **Análise do Adversário:** Identificar pontos fortes e fracos do oponente usando dados e vídeo. Quais perfis de jogadores do nosso elenco se encaixam melhor para explorar/neutralizar o adversário?  
      - **Modelagem de Cenários:** Simular o impacto de diferentes combinações de jogadores com base em dados históricos e táticos.  
     
3. **Integração com a Comissão Técnica:**  
   
      - **Reuniões Estratégicas:** Apresentação dos insights dos dados para o treinador e auxiliares. Discussão sobre como os achados se alinham (ou não) com a observação em treinos e jogos.  
      - **O Peso do "Olhômetro" e Intangíveis:** Como fatores não quantificáveis (liderança, comunicação, momento psicológico, entrosamento, experiência) são ponderados junto aos dados. A decisão final é *sempre* do treinador, informado pelos dados.

4\. **Feedback Pós-Jogo:** Analisar se as escolhas baseadas em dados funcionaram, refinar modelos e processos.

### IV. Exemplo Prático:

1. **Manchester City (Sob Guardiola):**  
      * **Foco:** Ênfase em dados táticos e posicionais. Métricas relacionadas ao controle de posse, passes em zonas específicas, pressão coordenada, ocupação de espaços ("jogo de posição"). A escolha dos jogadores muitas vezes depende de quem melhor executa funções táticas complexas exigidas contra um adversário específico, algo que a análise de dados (combinada com vídeo) ajuda a identificar.  
      * **Referência:** Livros sobre Guardiola (ex: *"Pep Confidential"* de Martí Perarnau), análises táticas detalhadas (Tifo Football/IRL no YouTube, The Athletic), artigos sobre o City Football Group e seu investimento em análise.

Fonte: [https://www.goodreads.com/book/show/22400946-pep-confidential/](https://www.goodreads.com/book/show/22400946-pep-confidential/)
<br>

### V. Desafios, Limitações e a Arte do Treinador

1. **Qualidade e Disponibilidade dos Dados:** Nem todos os clubes têm acesso aos mesmos dados (especialmente tracking data). A qualidade da coleta pode variar.  
2. **Contexto é Rei:** Uma métrica isolada pode enganar. O desempenho é influenciado pelo sistema tático, qualidade dos companheiros, nível do adversário, situação do jogo.  
3. **Risco de Supervalorização/Interpretação Equivocada:** Correlação não implica causalidade. Modelos podem ter vieses. Achar que "os números não mentem" é perigoso.  
4. **O Fator Humano e Intangível:** Liderança, resiliência, entrosamento, capacidade de decisão sob pressão – aspectos difíceis de quantificar, mas cruciais, que o treinador avalia diariamente.  
5. **Amostragem Pequena:** No futebol, poucos gols/eventos decisivos ocorrem por jogo. Métricas podem levar tempo para estabilizar.  
6. **Comunicação:** A habilidade dos analistas em comunicar insights complexos de forma clara e acionável para a comissão técnica é vital.

### VI. Conclusão e Perspectivas Futuras

1. **Síntese:** A análise de dados transformou a forma como as escalações são pensadas. É uma ferramenta indispensável para otimizar o desempenho físico, técnico e tático. No entanto, ela *complementa*, não substitui, a expertise do treinador, a observação direta e a compreensão das dinâmicas humanas do jogo. A decisão final é uma *fusão* de arte e ciência.

2. **O Futuro:**  
      * **Inteligência Artificial e Machine Learning:** Modelos preditivos mais sofisticados para risco de lesão, previsão de desempenho, identificação de padrões táticos complexos em tempo real.  
      * **Integração de Dados Biométricos e Cognitivos:** Monitoramento ainda mais detalhado do estado do jogador (se questões éticas e de privacidade forem resolvidas).  
      * **Análise Automatizada de Vídeo:** Extração automática de eventos táticos e dados de posicionamento a partir de imagens.  
      * **Feedback em Tempo Real:** Possibilidade de ajustes táticos e de pessoal durante o jogo baseados em dados ao vivo (já começando a ser explorado).  
      * **Democratização:** Ferramentas e dados ficando mais acessíveis para clubes de menor porte.

## Bibliografia

> [1]<a id=REF1></a> **SPORTS DATA CAMPUS.** Análise de desempenho no futebol. *Sports Data Campus*, [s.d.]. Disponível em: [https://sportsdatacampus.com/analise-de-desempenho-no-futebol/](https://sportsdatacampus.com/analise-de-desempenho-no-futebol/). Acesso em: 30 abr. 2025.
>
> [2]<a id=REF2></a> **AQUINO, R. L. T. de; COSTA, V. T. da; BARBOSA, G. F. et al.** Controle de carga no treinamento do atleta de alto rendimento: uma revisão sistemática. *ResearchGate*, 2024. Disponível em: [https://www.researchgate.net/publication/389833668_Controle_de_carga_no_treinamento_do_atleta_de_alto_rendimento_uma_revisao_sistematica](https://www.researchgate.net/publication/389833668_Controle_de_carga_no_treinamento_do_atleta_de_alto_rendimento_uma_revisao_sistematica). Acesso em: 30 abr. 2025.
>
> **DEEPMIND.** Game plan: what AI can do for football. *DeepMind Blog*, 2022. Disponível em: [https://deepmind.google/discover/blog/game-plan-what-ai-can-do-for-football/](https://deepmind.google/discover/blog/game-plan-what-ai-can-do-for-football/). Acesso em: 30 abr. 2025.
>
> **GOOGLE SCHOLAR.** Artificial intelligence sports analytics football. *Google Scholar*, [s.d.]. Disponível em: [https://scholar.google.com/scholar?q=artificial+intelligence+sports+analytics+football.](https://scholar.google.com/scholar?q=artificial+intelligence+sports+analytics+football.) Acesso em: 30 abr. 2025.

[Link para o documento de organização](https://docs.google.com/document/d/18EK2Og0RotStmt8G-Gqv17C8Qk32VYvzG4ybkhcFcFk/edit?usp=sharing)