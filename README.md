**Análise Experimental com Cilindros de PLA e Integração de Inteligência Artificial**

Este repositório apresenta o desenvolvimento de um projeto de iniciação científica focado na análise experimental de amostras cilíndricas de PLA, integrando métodos estatísticos, aprendizado de máquina supervisionado e não supervisionado para identificação de defeitos internos não visíveis externamente.
O estudo parte de dados experimentais reais provenientes de ensaios mecânicos destrutivos, explorando relações entre variáveis geométricas, físicas e mecânicas para detectar comportamentos atípicos associados a falhas estruturais internas.

**Contexto do Projeto**
A manufatura aditiva em polímeros, como o PLA, pode gerar defeitos internos difíceis de identificar por inspeção visual. Esses defeitos impactam diretamente a resistência mecânica das peças e comprometem sua confiabilidade estrutural.
Neste contexto, o projeto propõe o uso de ciência de dados e inteligência artificial como ferramentas auxiliares ao controle de qualidade, permitindo a identificação de amostras suspeitas a partir de padrões estatísticos e comportamentais dos dados experimentais.

**Objetivos** :
- Analisar estatisticamente dados experimentais de cilindros de PLA
- Investigar correlações entre variáveis geométricas, físicas e mecânicas
- Identificar amostras com comportamento mecânico anômalo
- Detectar defeitos internos não observáveis externamente
- Comparar abordagens supervisionadas e não supervisionadas
- Gerar uma lista objetiva de amostras suspeitas para validação técnica
- Construir um pipeline de análise reprodutível e interpretável

**Conjunto de Dados**
Os dados utilizados estão no formato CSV e contêm as seguintes variáveis:
- ID - Identificador da amostra
- diametro - Diâmetro do cilindro
- altura - Altura do cilindro
- massa - Massa da amostra
- resistencia - Resistência mecânica à ruptura

**Observações importantes**
A variável resistência pode conter valores nulos ou a string "FALHA"
Algumas amostras apresentam falha total no ensaio
Os defeitos internos não são visíveis externamente

**Metodologia**
O projeto é estruturado nas seguintes etapas:
- Limpeza e pré-processamento dos dados
- Tratamento de valores ausentes e falhas de ensaio
- Análise exploratória de dados (EDA)
- Visualização estatística com histogramas, boxplots e gráficos de dispersão
- Análise de correlação entre variáveis
- Regressão linear e análise de resíduos
- Engenharia de atributos (densidade aparente, resistência específica)
- Classificação supervisionada
- Support Vector Machine (SVM)
- Árvore de Decisão
- Aprendizado não supervisionado
- Isolation Forest para detecção de anomalias
- Integração dos resultados para identificação de amostras suspeitas
- Exportação dos IDs suspeitos para validação experimental

**Técnicas e Modelos Utilizados**

- Estatística descritiva
- Regressão linear
- Análise de resíduos
- Classificação supervisionada
- Detecção de outliers
- Aprendizado não supervisionado
- Engenharia de atributos
- Avaliação de modelos com métricas clássicas

**Tecnologias e Bibliotecas**

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
