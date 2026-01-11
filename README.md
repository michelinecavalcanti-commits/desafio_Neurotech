# 📊 Análise de Crédito  
**Projeto de Análise de Dados | Portfólio Profissional**

## 🧑‍💼 Identificação do Projeto

| Item | Descrição |
|-----|-----------|
| 👤 Autora | Micheline Jeane Lima Cavalcanti |
| 📌 Projeto | Análise de Crédito |
| 📅 Data de entrega | 31 de julho de 2025 |
| 🎓 Contexto | Projeto educacional – *Vem pra Neuro, Mulher!* |
| 🏢 Origem dos dados | Télos & Neurotech (uso educacional) |

---

## 🗂️ Bases de Dados

### 📥 Bases recebidas
- `CADASTRAL.csv`
- `COMPRAS.csv`
- `CAMPANHAS.csv`
- `PRE_NEGADOS.csv`
- `RECLAMACOES.csv`
- `LIQUIDADADOS.csv`

### 📊 Bases utilizadas na análise
- `CADASTRAL.csv`
- `PRE_NEGADOS.csv`
- `LIQUIDADADOS.csv`

---

## 🎯 Contexto e Objetivo

Este projeto teve como objetivo analisar o **comportamento de clientes** em relação à:

- concessão de crédito  
- inadimplência  
- desempenho financeiro  

### Perguntas norteadoras:
- Qual o perfil dos clientes com maior propensão à inadimplência?
- Quais fatores influenciam a reprovação de crédito?
- Como reduzir riscos e melhorar a concessão de crédito?

### Hipóteses investigadas:
- Score baixo, renda insuficiente e inconsistências cadastrais são os principais impeditivos.
- Políticas de crédito personalizadas reduzem inadimplência e aumentam faturamento.

---

## 🔐 Fontes de Dados e LGPD

Os dados foram utilizados **exclusivamente para fins educacionais**, respeitando a LGPD:

- Não contêm dados sensíveis ou identificadores diretos  
- Uso restrito ao contexto acadêmico  
- Finalidade legítima de aprendizado e simulação de cenários reais  

📜 **Lei nº 13.709/2018 – LGPD**


## 🔄 Processo de Análise de Dados

### ETL – Extração, Transformação e Limpeza
- Padronização de colunas (`cliente_id`, campos numéricos)
- Tratamento de valores nulos e inconsistentes
- Conversão de tipos (`score_inicial`, `renda_mensal`)

### EDA – Análise Exploratória
- Estatísticas descritivas (médias, totais, proporções)
- Comparações entre clientes aprovados, reprovados e inadimplentes
- Análises por:
  - gênero
  - escolaridade
  - faixa etária
  - renda
  - ocupação
  - score
  - estado civil

### Cruzamento de Variáveis
- Score × renda × concessão de crédito
- Perfis de clientes adimplentes vs. inadimplentes (Top 50 e Top 100)
- Motivos de negativa e tentativas subsequentes

---

## 🛠️ Ferramentas Utilizadas

- 🐍 **Google Colab** — limpeza e análise dos dados  
- 📊 **Google Sheets** — validação inicial e padronização  
- 📽️ **Google Slides** — apresentação final  

### Visualizações
- Gráficos de barras (inadimplência por faixa etária, ocupação e score)
- Tabelas resumo com médias e percentuais
- Comparativos entre grupos de clientes

---

## 💡 Insights e Recomendações

### 🔎 Principais Descobertas

**1️⃣ Motivos de Negativa**
- 30% → Renda insuficiente  
- 20% → Inconsistência cadastral  
- 15% → Documentação incompleta  
➡️ Mais de **60%** relacionados a cadastro e documentação

**2️⃣ Perfil dos Inadimplentes (Top 50)**
- 64% masculino | 62% casado(a)
- 54% ensino médio | 18% vendedor(a)
- Score médio: **467**
- Renda média: **R$ 2.381,00**

**3️⃣ Perfil dos Adimplentes (Top 50)**
- 62% feminino | 44% solteiro(a)
- 46% pós-graduado(a) | 56% servidor(a) público(a)
- Score médio: **553**
- Renda média: **R$ 5.047,00**

**4️⃣ Renegociação**
- 75% das novas solicitações aprovadas
- 31% superaram o critério de renda insuficiente

**5️⃣ Concentração de Inadimplência**
- 60% da base adimplente
- 33% com histórico de inadimplência

---

### 📌 Recomendações Estratégicas
- Validação de dados em tempo real no cadastro
- Alertas automáticos para pendências documentais
- Limites iniciais menores com progressão por histórico
- Campanhas de reoferta personalizadas
- Educação financeira segmentada
- Programa de recompensas para bons pagadores

---

## 📚 Aprendizados e Reflexões

### Aprendizados
- Importância do cruzamento entre variáveis demográficas e financeiras
- Impacto direto da limpeza de dados nos resultados
- Transformação de dados brutos em decisões estratégicas

### Desafios
- Integração de múltiplas bases via `cliente_id`
- Padronização manual em etapas no Google Sheets
- Tratamento cuidadoso de outliers

### O que faria diferente?
- Padronização mais rígida desde a entrada dos dados
- Testes com dados sintéticos e divisão 70/30 antes da integração total

---

## 📎 Referências
- Dados: Télos & Neurotech – *Vem pra Neuro, Mulher!*  
- Google Colab: https://colab.research.google.com  
- Google Sheets: https://sheets.google.com  
- LGPD – Lei nº 13.709/2018  
- Material do curso de Formação em Análise de Dados – Télos/Neurotech

