# **Uso de Dados na Análise Tática Moderna**

---

## **1\. Evolução histórica da análise tática**

### **1950–1980  │ Primeiros experimentos manuais**

* **1950s – Charles Reep** registra toque‑a‑toque em fichas de papel, gerando a primeira base quantitativa sobre padrões de ataque e probabilidade de gol.
* Estudos focavam em contagens simples (passes, chutes) e relatórios qualitativos, limitados pela tecnologia de filmagem.

### **1990–2005  │ Digitalização e sistemas de vídeo**

* **1995 – Prozone** lança o primeiro sistema comercial de rastreamento por câmera no futebol inglês.
* Clubes da Premier League e seleções de rúgbi usam Prozone para ajuste tático e recrutamento, inspirando “Moneyball”.

### **2005–2015  │ Era dos sistemas de rastreamento ótico & GPS**

* **2005 – SportVU** nasce em Israel; em 2013, adotado pela NBA, mostrando potencial de rastreamento em tempo real.
* Plataformas como Amisco, Tracab e Catapult ampliam sensores e wearables.
* **2015 – IFAB/FIFA** legaliza EPTS em partidas oficiais.

### **2012–2020  │ Métricas avançadas e dados abertos**

* **2012 – Expected Goals (xG)** populariza modelos de probabilidade de gol.
* Surgem modelos de valor de ação (VAEP, EPV) combinando evento e rastreamento.
* **2018 – StatsBomb Open Data** democratiza dados de eventos.

### **2020–2025  │ IA, big data e volumetria 3D**

* **2020 – Second Spectrum** fornece métricas táticas em tempo real na Premier League.
* **Intel True View** traz replay volumétrico 3D para LaLiga, NFL e UCL.
* Edge/5G e XAI transformam dados brutos em insights.

---

## **2\. Tipos de dados disponíveis**

| Grupo | Origem | Exemplos | Informação tática |
| ----- | ----- | ----- | ----- |
| Rastreamento | Câmeras, GPS, UWB | posição, velocidade, acel. | formações, zonas de pressão |
| Evento | Opta, Wyscout, StatsBomb | passes, chutes, faltas | sequência de ações com bola |
| Vídeo/Imagem | Transmissão, drones | frames sincronizados | contexto visual, gestos |
| Biométricos | Wearables, GPS | FC, distância, impactos | fadiga, risco de lesão |

---

## **3\. Métricas tradicionais × avançadas**

### **3.1 Por que ultrapassar contagens?**

Contagens (gols, assistências, % de passe) são intuitivas, mas não capturam contexto espacial ou tático. Métricas avançadas estimam valor e consequência de ações.

### **3.2 Contagens & Taxas**

| Métrica | Descrição | Limitação |
| ----- | ----- | ----- |
| Gols / Assistências | Eventos finais de ataque | Alta variância |
| % Passe | Passes certos ÷ totais | Ignora risco e impacto |
| Chutes a gol | Finalizações no alvo | Qualidade ignorada |
| Desarmes/Intercept. | Ações defensivas bem‑sucedidas | Sem contexto espacial |

### **3.3 Valor de Ação/Posse**

| Acrônimo | Essência |
| ----- | ----- |
| xG | Prob. de gol de um chute |
| xA | Prob. de gol resultante de um passe |
| xT | Valor da posse em células (cadeia de Markov) |
| VAEP | Δ prob. gol contra/pro gol em sequência de ações |
| EPV | Valor esperado da posse a cada frame (tracking 25 Hz) |

### **3.4 Pressão & Defesa**

| Métrica | Cálculo |
| ----- | ----- |
| PPDA | Passes permitidos ÷ ações defensivas altas |
| BDP | Variação da % passe rival na construção |
| D‑VAEP | Δ prob. gol adversário por ação defensiva |

### **3.5 Clustering & Perfis**

* K‑Means/MiniBatch para perfis táticos.
* PCA \+ t‑SNE/UMAP para visualização de alta dimensão.
* Roles dinâmicos via tracking.

---

## **4\. Fluxo de processamento e modelagem**

Coleta & Integração \--\> Armazenamento \--\> Pré-processamento \--\> Feature Engineering \--\> Modelagem \--\> Visualização

*Diagrama interativo disponível no dashboard interno.*

---

## **5\. Modelos analíticos, MCMC e otimização**

### **5.1 Modelos estatísticos & heurísticos**

* Regressão logística/LASSO multinomial para P(vitória).
* Árvores de decisão e Gradient Boosting para eventos críticos.
* Random Forest/XGBoost para importância de features.
* Meta‑heurísticas (GA, GRASP, ALNS) e CP‑SAT para escalações.
* Deep RL/MARL para políticas táticas em ambientes parciais.

### **5.2 Inferência Bayesiana & MCMC**

* **MCMC**: exploração aleatória que converge à distribuição posterior.
* **ESS**: calcula tamanho efetivo de amostras para regularização e early-stopping.
* **Hamiltonian MC/NUTS**, SGLD/SGHMC e inferência variacional para acelerar.
* Priors hierárquicos e sequential MC para evitar overfitting.

#### **Demonstrações Visuais**

### **5.3 Feature Engineering Avançado**

* Terraint embedding (VAE), sinergia (Elo/TrueSkill).
* Zone control, entropia de crença inimiga, momentum.
* Embeddings temporais (GRU/TCN) e priors SGLD.

---

## **6\. Análise de desempenho individual**

* Fusão de evento \+ rastreamento valoriza cada ação.
* Indicadores físicos (sprints, cargas) para fadiga.
* Clustering de substitutos e perfis.

---

## **7\. Aplicações táticas em tempo real**

* Dashboards ao vivo e alertas de fadiga.
* Simulações contrafactuais e IA prescritiva.

---

## **8\. Desafios atuais**

* Cobertura desigual em ligas menores.
* Latência e volume nos pipelines.
* Viés algorítmico e interpretabilidade.

---

## **9\. Tendências futuras**

* Edge/5G e integração de wearables avançados.
* Modelos XAI e assistentes conversacionais.
* Realidade aumentada para técnicos.

---

## **10\. Conclusões**

* Evolução de contagens manuais a pipelines de Big Data.
* Sinergia de múltiplas fontes para visão holística.
* Técnicas avançadas trazem vantagem competitiva.

---

## **11\. Diagramas e Glossário Visual**

### **11.1 Heatmap de Métricas**

**Figura 3\.** Mapa térmico combinando xG, PPDA e VAEP.

### **11.2 Fluxo de Processamento (Seção 4\)**

**Figura 4\.** Diagrama resumido das etapas.

### **11.3 Analogias Práticas**

| Termo | Analogia |
| ----- | ----- |
| MCMC | Explorar ruas aleatórias até achar a praça central |
| VAEP | Avaliar cada passe como pontos em um tabuleiro |
| MARL | Motoristas de entrega aprendendo rotas em conjunto sem mapa completo |

---

## **12\. Recomendações Finais**

### **Para Leitores Técnicos**

* **Calcular ESS**: use autocorrelação das cadeias para estimar ESS; target ≥ 200\.
* **Referências Avançadas**: Gelman et al. (2013) “Bayesian Data Analysis”, Betancourt (2017) “A Conceptual Introduction to HMC and NUTS”.
* **Detalhes Metodológicos**: implantar SGLD em GPU e monitorar gradients para estabilidade.

### **Para Gestores (SWOT)**

| Tecnologia | Forças | Fraquezas | Oportunidades | Ameaças |
| ----- | ----- | ----- | ----- | ----- |
| Intel True View | Visão volumétrica 3D detalhada | Alto custo de implementação | Marketing diferenciado | ROI incerto em ligas menores |
| Second Spectrum | Métricas em tempo real | Dependência de parcerias | Monetização via licenças | Barreiras regulatórias |

### **Para Disseminação Pública**

* **Infográficos & Vídeos**: sintetizar Figuras 3 e 4 em animações curtas para redes sociais.
* **Apresentações Executivas**: slides com pontos-chave e diagramas simplificados.
* **Versões Resumidas**: PDFs de 1 página com bullet points e gráficos interativos no web app.

---

## **13\. Referências Selecionadas**

> Internal docs: *Evolução da análise tática*, *Dados usados na análise tática moderna*, etc.
>
> Gelman, A. et al. “Bayesian Data Analysis” (3rd ed., 2013).
>
> Betancourt, M. “A Conceptual Introduction to HMC and NUTS” (2017).
>
> StatsBomb, The Analyst, Coaches’ Voice, FootSci articles (2023–2024).

[Link para o documento de organização](https://docs.google.com/document/d/1K23WhHtLVzY9GAIbjBjsXnqs8-OQjaSJjINWELJOY8k/edit?usp=sharing)