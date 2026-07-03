# 👥 Dashboard de RH — Power BI

**Stack:** Power BI (Modelo de Dados, DAX, Relatório Interativo)
**Base de dados:** Excel — 494 funcionários com dados de folha, avaliação e histórico
**Objetivo:** Monitorar a saúde do capital humano da empresa — turnover, folha salarial, avaliações de desempenho, horas extras e férias acumuladas — em um painel interativo para o time de RH e liderança

---

## 📖 O Contexto

Esta base simula o cadastro completo de RH de uma empresa com **494 funcionários** distribuídos em **5 áreas** e **5 níveis hierárquicos**. Cada registro traz dados pessoais, contratuais (admissão, demissão, salário, benefícios) e de desempenho (avaliação geral + 5 competências individuais: trabalho em equipe, liderança, comunicação, iniciativa e organização).

---

## 🗂️ Estrutura dos Dados

| Campo | Descrição |
|---|---|
| ID RH | Identificador único do funcionário |
| Nome Completo | Nome do colaborador |
| Estado Civil / Sexo | Dados demográficos |
| Data de Nascimento | Para cálculo de faixa etária |
| Data de Contratação / Demissão | Histórico contratual e cálculo de turnover |
| Salário Base / Impostos / Benefícios / VT / VR | Composição da folha de pagamento |
| Cargo / Nível / Área | Estrutura hierárquica |
| Férias Acumuladas / Horas Extras | Indicadores operacionais |
| Avaliação + 5 Competências | Desempenho individual (escala 0-10) |

---

## 📊 Principais KPIs

### 👤 Visão Geral do Quadro

| Indicador | Valor |
|---|---|
| Total de funcionários | 494 |
| Funcionários ativos | 432 |
| Funcionários desligados | 62 |
| **Taxa de turnover** | **12,6%** |
| Tempo médio de empresa (ativos) | 14,1 anos |
| Funcionário mais antigo | 24,0 anos de casa |

**Insight:** Taxa de turnover de 12,6% está acima do benchmark saudável para empresas brasileiras (8-10%). Com um tempo médio de 14 anos de empresa, o quadro é experiente — mas o turnover elevado pode estar concentrado em níveis específicos.

---

### 💰 Folha Salarial

| Indicador | Valor |
|---|---|
| Folha total | R$ 3.449.234,00 |
| Salário médio geral | R$ 6.982,26 |
| Salário mínimo | R$ 800,00 |
| Salário máximo | R$ 25.452,00 |

### Salário Médio por Nível

| Nível | Salário Médio |
|---|---|
| Diretor | R$ 23.881,80 |
| Gerente | R$ 15.116,70 |
| Coordenador | R$ 10.986,15 |
| Analista | R$ 6.472,90 |
| Estagiário | R$ 1.387,95 |

### Salário Médio por Área

| Área | Salário Médio |
|---|---|
| Logística | R$ 7.489,84 |
| Comercial | R$ 7.113,88 |
| Financeiro | R$ 6.993,88 |
| Operações | R$ 6.724,05 |
| Administrativo | R$ 6.674,46 |

**Insight:** Logística tem o maior salário médio entre as áreas — possivelmente por concentrar mais cargos de coordenação e gerência. A diferença entre Diretor (R$ 23.881) e Estagiário (R$ 1.387) é de **17x** — amplitude salarial expressiva.

---

### 📊 Distribuição por Gênero

| Gênero | Qtd | Participação |
|---|---|---|
| Masculino | 274 | 55,5% |
| Feminino | 220 | 44,5% |

---

### ⭐ Avaliação Média por Nível

| Nível | Avaliação Média |
|---|---|
| Diretor | 8,60 |
| Analista | 8,29 |
| Estagiário | 8,27 |
| Gerente | 8,19 |
| Coordenador | 8,11 |

**Insight:** Diretores têm a maior avaliação média (8,60), o que é esperado. O achado contraintuitivo: **Estagiários (8,27) superam Gerentes (8,19) e Coordenadores (8,11)** — pode indicar que os estagiários são avaliados com critérios diferentes, ou que há uma camada de gestão média com desempenho relativamente mais baixo.

---

### ⏰ Horas Extras por Área

| Área | Total Horas Extras |
|---|---|
| Administrativo | 11.490 h |
| Operações | 10.631 h |
| Comercial | 10.384 h |
| Logística | 9.882 h |
| Financeiro | 7.987 h |

**Insight:** Administrativo lidera em horas extras apesar de ter o menor salário médio entre as áreas — combinação que pode indicar sobrecarga e risco de insatisfação.

---

### 🏖️ Férias Acumuladas (Alerta Crítico)

| Indicador | Valor |
|---|---|
| Funcionários com férias > 30 dias | **262 (53% do quadro)** |
| Maior acúmulo individual | 60 dias — Jeferson Ramos |

**Insight:** Mais da metade do quadro ativo tem férias acumuladas acima de 30 dias — passivo trabalhista relevante. Com 432 ativos e 262 com férias vencidas, isso representa risco financeiro e jurídico real pra empresa.

---

## 🧠 Sobre as Habilidades Aplicadas

Nível: **intermediário em Excel e Power BI** — modelagem de dados de RH, construção de indicadores de capital humano (turnover, composição de folha, avaliação de desempenho) e visualização interativa com filtros por área, nível, gênero e período. Aplicado via DAX para cálculo de taxa de turnover, tempo médio de empresa, distribuição salarial e rankings de desempenho.

---

## 🎥 Demonstração

![Dashboard em funcionamento](dashboard.gif)

---

## 📁 Estrutura do Projeto

```
Dashboard-RH-PowerBI/
├── BaseFuncionarios.xlsx   # Base com 494 funcionários
├── dashboard.gif           # Demonstração do relatório interativo
└── README.md               # Este arquivo
```

---

## 🚀 Como Reproduzir

1. Baixe o arquivo `BaseFuncionarios.xlsx`
2. Importe no Power BI Desktop (Obter Dados → Excel)
3. Construa as medidas DAX: taxa de turnover, salário médio por área/nível, avaliação média, total de horas extras
4. Monte os visuais com filtros por área, nível hierárquico e gênero

---

📫 **Contato:** [LinkedIn](https://www.linkedin.com/in/simaosantana-a744372a7) · simaojoaosantana@gmail.com
