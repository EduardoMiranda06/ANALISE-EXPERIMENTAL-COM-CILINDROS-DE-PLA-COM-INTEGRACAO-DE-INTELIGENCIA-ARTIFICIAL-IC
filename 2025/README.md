# 📁 Base de Dados 2025 – Análise Experimental de Cilindros de PLA

Esta pasta contém as análises referentes à **base experimental de 2025**, utilizada no projeto de Iniciação Científica *Análise Experimental com Cilindros de PLA com Integração de Inteligência Artificial*.

Diferentemente da base anterior (2024), esta base introduz **um novo fator experimental**: o **tratamento térmico por recozimento**, permitindo análises comparativas e inferências estatísticas sobre seu efeito na resistência mecânica das amostras.

---

## 🎯 Objetivos da Análise (Base 2025)

Os objetivos desta etapa do projeto são:

- Avaliar o impacto do **tratamento térmico (recozimento)** no aumento da resistência mecânica do PLA  
- Comparar amostras **recozidas vs não recozidas** em termos de:
  - resistência
  - dispersão
  - ocorrência de falhas
- Identificar **outliers e amostras estruturalmente defeituosas**
- Detectar **IDs suspeitos**, mesmo em peças submetidas ao tratamento térmico
- Integrar técnicas de:
  - análise estatística
  - aprendizado de máquina supervisionado
  - aprendizado não supervisionado (detecção de anomalias)

---

## 🧪 Variáveis da Base de Dados

A base de 2025 contém as seguintes colunas:

- **ID** – identificador único da amostra  
- **Diâmetro (mm)** – diâmetro do cilindro  
- **Altura (mm)** – altura do cilindro  
- **Massa (g)** – massa da amostra  
- **Resistência (kgf)** – carga máxima suportada no ensaio  
- **Recozidos** – indica se a amostra passou por tratamento térmico (`SIM` ou `NÃO`)

---

## ⚠️ Peculiaridades e Desafios da Base

Esta base apresenta características importantes que exigem tratamento específico dos dados:

### 🔹 Massa (g)
- Existem amostras com **massa igual a 0**, o que é fisicamente inválido
- Esses valores são tratados como ausentes (NaN) para evitar vieses estatísticos

### 🔹 Resistência (kgf)
- Algumas amostras apresentam o valor **"FALHA"**
- Esse valor indica **falha total no ensaio mecânico**
- As falhas são separadas das resistências numéricas e utilizadas como informação crítica na identificação de defeitos

### 🔹 Recozidos
- Variável categórica com valores `SIM` e `NÃO`
- Convertida para variável binária para:
  - análise estatística
  - regressão
  - aprendizado de máquina

---

## 📊 Estratégia Analítica

As análises desenvolvidas nesta pasta incluem:

- Análise exploratória com visualizações estatísticas
- Comparação de distribuições entre recozidos e não recozidos
- Testes estatísticos para avaliar a efetividade do tratamento térmico
- Regressão linear com variável de tratamento
- Análise de resíduos para detecção de defeitos internos
- Detecção de anomalias via Isolation Forest
- Modelos supervisionados (SVM e Árvore de Decisão)
- Geração de lista final de **IDs suspeitos para validação experimental**

---

## 🧠 Relevância Científica

A base de 2025 permite responder perguntas centrais do projeto, como:

- O recozimento aumenta significativamente a resistência do PLA?
- O tratamento térmico reduz a ocorrência de falhas estruturais?
- Ainda existem defeitos internos mesmo após o tratamento?
- Quais amostras devem ser investigadas experimentalmente?

---

📌 *Esta etapa representa a integração entre ciência dos materiais, estatística aplicada e inteligência artificial, elevando o projeto a um nível experimental e analítico mais avançado.*