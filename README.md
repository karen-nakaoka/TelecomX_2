# 📊 Previsão de Evasão de Clientes (Churn Prediction)

## 📌 Sobre o Projeto

A evasão de clientes (churn) é um dos principais desafios enfrentados por empresas de telecomunicações, pois representa perda direta de receita e aumento dos custos de aquisição de novos clientes.

Este projeto tem como objetivo **analisar os fatores que influenciam a evasão de clientes** e construir modelos de **Machine Learning** capazes de prever quais clientes apresentam maior risco de cancelamento.

A partir dessa análise, é possível apoiar decisões estratégicas e desenvolver **estratégias de retenção de clientes**.

---

# 🧠 Objetivos

- Analisar o comportamento de clientes de uma empresa de telecomunicações
- Identificar fatores associados à evasão de clientes
- Construir modelos de machine learning para prever churn
- Comparar o desempenho de diferentes algoritmos
- Interpretar as variáveis mais importantes para o cancelamento

---

# 📂 Dataset

O conjunto de dados utilizado contém **7043 clientes** e **24 variáveis**, incluindo:

- Informações demográficas
- Serviços contratados
- Tipo de contrato
- Forma de pagamento
- Gastos mensais e totais
- Indicador de evasão do cliente

A variável alvo do problema é:

**Evasão**
- 0 → Cliente permaneceu  
- 1 → Cliente cancelou o serviço

---

# ⚙️ Tecnologias utilizadas

Este projeto foi desenvolvido em **Python**, utilizando as seguintes bibliotecas:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

O notebook foi desenvolvido utilizando **Google Colab**.

---

# 🔎 Etapas do Projeto

## 1️⃣ Extração e entendimento dos dados

- Importação do dataset
- Análise inicial da estrutura dos dados
- Verificação de valores nulos
- Identificação das variáveis disponíveis

---

## 2️⃣ Preparação dos dados

Foram realizadas as seguintes etapas:

- Remoção de colunas irrelevantes
- Separação entre variáveis preditoras e variável alvo
- Conversão de variáveis categóricas utilizando **One-Hot Encoding**
- Padronização de variáveis numéricas

---

## 3️⃣ Análise exploratória

Foram realizadas análises para entender o comportamento dos clientes:

- Proporção de evasão
- Matriz de correlação
- Análise visual com **boxplots**
- Identificação de possíveis fatores associados ao churn

---

## 4️⃣ Modelagem preditiva

Os dados foram divididos em:

- **80% treino**
- **20% teste**

Foram treinados dois modelos de classificação:

### Regressão Logística

Modelo linear amplamente utilizado em problemas de classificação binária, conhecido por sua interpretabilidade.

### Random Forest

Algoritmo baseado em **conjunto de árvores de decisão**, capaz de capturar relações mais complexas entre variáveis.

---

# 📈 Avaliação dos Modelos

Os modelos foram avaliados utilizando:

- Acurácia
- Precisão
- Recall
- F1-score
- Matriz de confusão

### Resultados

| Modelo | Acurácia | Precisão | Recall | F1-score |
|------|------|------|------|------|
| Regressão Logística | 0.79 | 0.63 | 0.52 | 0.57 |
| Random Forest | 0.78 | 0.62 | 0.46 | 0.53 |

A **Regressão Logística apresentou desempenho ligeiramente superior**, especialmente nas métricas de **recall e F1-score**.

---

# 🔑 Principais fatores associados à evasão

A análise dos modelos identificou alguns fatores importantes relacionados ao cancelamento de clientes:

Maior probabilidade de evasão:

- Clientes com **internet Fiber optic**
- Forma de pagamento **Electronic check**
- **Gasto mensal elevado**
- Clientes com **menos tempo de contrato**

Menor probabilidade de evasão:

- **Contratos de longo prazo**
- Clientes com **maior tempo de permanência**
- Clientes com **serviços adicionais**, como suporte técnico e segurança online

---

# 💡 Possíveis estratégias de retenção

Com base nos resultados obtidos, algumas estratégias podem ser consideradas:

- Criar programas de retenção para **clientes nos primeiros meses de contrato**
- Oferecer **benefícios para contratos de longo prazo**
- Monitorar clientes com **maior risco de churn**
- Incentivar **formas de pagamento automáticas**
- Melhorar a experiência de clientes com **internet Fiber optic**

---

# 📊 Conclusão

Este projeto demonstrou como técnicas de **análise de dados e machine learning** podem ser utilizadas para identificar clientes com maior risco de evasão.

A utilização desses modelos permite que empresas atuem de forma **proativa**, desenvolvendo estratégias de retenção e melhorando o relacionamento com seus clientes.

---

# 🚀 Possíveis melhorias futuras

- Testar novos modelos de machine learning (SVM, XGBoost)
- Aplicar técnicas de balanceamento de classes
- Realizar otimização de hiperparâmetros
- Construir um sistema de previsão em produção
- Criar dashboards interativos para monitoramento do churn
