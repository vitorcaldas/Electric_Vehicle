# Electric_Vehicle

# ⚡ Análise e Exploração de Dados: Veículos Elétricos (EV Analytics)

## 📌 Visão Geral do Projeto
Este projeto consiste em uma Análise Exploratória de Dados (EDA) aplicada a um conjunto de dados sobre **Veículos Elétricos (EVs)**. O objetivo é compreender o panorama atual do mercado, analisando desde a eficiência energética, saúde da bateria e custos operacionais até aspectos econômicos como depreciação e custo de manutenção.

---

## 📊 Estrutura do Dataset
O conjunto de dados (`electric_vehicle_analytics.csv`) possui **3.000 registros** e **25 colunas**, sem valores nulos (dados completos).

### Principais Variáveis Analisadas:
- **Identificação & Categoria:** `Vehicle_ID`, `Make` (Marca), `Model`, `Year`, `Region`, `Vehicle_Type`, `Usage_Type` (Pessoal, Frota, Comercial).
- **Desempenho & Bateria:** `Battery_Capacity_kWh`, `Battery_Health_%`, `Range_km`, `Charging_Power_kW`, `Charging_Time_hr`, `Charge_Cycles`, `Energy_Consumption_kWh_per_100km`.
- **Métricas de Condução:** `Mileage_km`, `Avg_Speed_kmh`, `Max_Speed_kmh`, `Acceleration_0_100_kmh_sec`, `Temperature_C`.
- **Sustentabilidade & Economia:** `CO2_Saved_tons`, `Maintenance_Cost_USD`, `Insurance_Cost_USD`, `Electricity_Cost_USD_per_kWh`, `Monthly_Charging_Cost_USD`, `Resale_Value_USD`.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas
A análise foi desenvolvida em **Python 3** (ambiente Google Colab) utilizando as seguintes bibliotecas:

- **Pandas:** Manipulação e estruturação dos dados (`DataFrame`).
- **NumPy:** Suporte a operações matemáticas e vetoriais.
- **Matplotlib & Seaborn:** Visualização de dados e geração de gráficos estatísticos.

---

## 🚀 Fluxo da Análise (EDA)

1. **Carregamento e Inspeção Inicial:**
   - Leitura do arquivo CSV via Pandas.
   - Verificação das primeiras linhas (`df.head()`).
   - Mapeamento dos tipos de dados (`df.info()`).

2. **Sanidade dos Dados & Cardinalidade:**
   - Checagem de dados ausentes (`df.isnull().sum()`), confirmando 0 valores nulos.
   - Contagem de valores únicos por variável (`df.nunique()`).

3. **Estatística Descritiva:**
   - Análise de dispersão, média, quartis e extremos (`df.describe()`).
   - *Insight preliminar:* A saúde média da bateria da frota é de **85%**, com valor de revenda médio de **$22.257,00**.

4. **Tendências de Mercado e Distribuições:**
   - Análise gráfica da distribuição percentual da saúde da bateria utilizando histogramas com estimativa de densidade de kernel (KDE).

---

## 📂 Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
