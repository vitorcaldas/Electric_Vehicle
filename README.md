# Electric_Vehicle

# 🚗 Análise de Veículos Elétricos (EV Analytics)

 O objetivo principal do projeto é entender as distribuições de capacidade de bateria, autonomia (*range*), custos operacionais (carregamento e manutenção), depreciação e o impacto ambiental (redução de emissões de CO₂) em diferentes regiões e categorias de uso.

---

## 📊 Visão Geral do Dataset

O dataset analisado (`electric_vehicle_analytics.csv`) é composto por **3.000 registos** e **25 colunas**, sem registos nulos.

### Principais Variáveis Analisadas:
- **Identificação e Categoria:** `Make`, `Model`, `Year`, `Region`, `Vehicle_Type` (SUV, Sedan, Hatchback, Truck), `Usage_Type` (Personal, Fleet, Commercial).
- **Desempenho e Bateria:** `Battery_Capacity_kWh`, `Battery_Health_%`, `Range_km`, `Charging_Power_kW`, `Energy_Consumption_kWh_per_100km`, `Max_Speed_kmh`, `Acceleration_0_100_kmh_sec`.
- **Fatores Financeiros e Ambientais:** `CO2_Saved_tons`, `Maintenance_Cost_USD`, `Insurance_Cost_USD`, `Electricity_Cost_USD_per_kWh`, `Monthly_Charging_Cost_USD`, `Resale_Value_USD`.

---

## 🔬 Principais Destaques e Resultados da EDA

1. **Qualidade dos Dados:**
   - **Tamanho do dataset:** 3.000 linhas × 25 colunas.
   - **Valores Ausentes:** 0 valores nulos em todas as colunas.
   - **Diversidade:** 10 fabricantes diferentes (`Make`), 23 modelos (`Model`), 4 regiões geográficas e 4 tipos de veículo.

2. **Métricas de Desempenho Médio:**
   - **Capacidade Média da Bateria:** ~74.81 kWh (variando de 30 kWh a 120 kWh).
   - **Autonomia Média (*Range*):** ~374.4 km (máximo de 713 km).
   - **Saúde da Bateria (*Battery Health*):** Média de 85.03% (com mínimo de 70%).
   - **Economia Média de CO₂:** ~15.02 toneladas por veículo.
   - **Valor Médio de Revenda:** ~$22.257,00 USD.

3. **Análises Bivariadas e Visuais:**
   - **Capacidade de Bateria por Tipo de Veículo:** Comparação da distribuição de capacidade entre SUVs, Sedans, Hatchbacks e Trucks.
   - **Autonomia por Região:** Análise de variação do alcance médio entre Ásia, Europa, América do Norte e Austrália.
   - **Custos Mensais de Carregamento:** Avaliação dos impactos de custo segundo o perfil de uso (*Commercial*, *Fleet*, *Personal*).
   - **Impacto Ambiental:** Distribuição da quantidade de CO₂ economizado agrupado por tipo de veículo.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

O projeto foi desenvolvido em **Python 3** no ambiente Google Colab, utilizando as seguintes bibliotecas:

- **[Pandas](https://pandas.pydata.org/):** Manipulação, limpeza e agregação de dados.
- **[NumPy](https://numpy.org/):** Operações numéricas e vetoriais.
- **[Seaborn](https://seaborn.pydata.org/):** Visualização estatística de dados (Boxplots, Violin plots).
- **[Matplotlib](https://matplotlib.org/):** Customização de gráficos e estruturas de figuras.
- **[scikit-learn](https://scikit-learn.org/):** Machine Learning, pré-processamento de dados (escalamento/codificação) e avaliação de modelos.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter o Python 3.x instalado, juntamente com as bibliotecas necessárias.

```bash
pip install numpy pandas seaborn matplotlib
