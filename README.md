# Atividade Prática — Análise de Dados no Setor de Energia

**Curso:** Ciência da Computação
**Disciplina:** Soluções em Energias Renováveis e Sustentáveis (SERS)
**Atividade:** Orange Data Mining, Python e Pandas

## Integrantes

- João Victor Canello Ferian - RM573295
- Lucas Klein - RM570029
- Gustavo Melo dos Santos - RM573562
- João Pedro Costenari Silva - RM572260

## Objetivo

Aplicar os procedimentos trabalhados em aula para preparar, inspecionar e analisar diferentes conjuntos de dados do setor de energia, relacionando cada operação realizada ao contexto do dataset.

## Entrega

Os exercícios de Python são resolvidos em um único notebook Python (`.ipynb`). A etapa no Orange Data Mining é usada para conhecer e preparar os dados (seleção de atributos, verificação de qualidade e amostragem) antes da análise no Python/Pandas.

## Dataset trabalhado por este grupo

**Dataset 1 — Appliances Energy Prediction (UCI)**

> Situação: a empresa de eficiência energética está analisando o comportamento de uma residência de baixo consumo. A equipe deseja identificar períodos de consumo elevado dos eletrodomésticos e observar quais condições de temperatura e umidade estavam presentes nesses momentos.

**Etapa A — Orange Data Mining**
- Carregar `energydata_complete.csv` com o widget File.
- Inspecionar os registros no Data Table e identificar atributos de consumo, temperatura e umidade.
- Usar Select Columns para manter `Appliances`, `lights`, pelo menos três atributos de temperatura e três de umidade.
- Verificar valores ausentes (o dataset do UCI não possui, mas a checagem faz parte do procedimento).
- Gerar uma amostra aleatória de 10% com Data Sampler.
- Exportar a amostra em CSV com Save Data.

**Etapa B — Python / Pandas**
- Carregar a amostra e apresentar `head()`, `shape`, `info()` e `describe()`.
- Renomear `Appliances` para `Consumo_Eletrodomesticos` e simplificar pelo menos três atributos ambientais.
- Determinar o maior consumo de eletrodomésticos registrado na amostra.
- Calcular um limiar de 70% do valor máximo e criar um DataFrame com os registros acima desse limite.
- Contar os registros selecionados e calcular o percentual que representam da amostra.
- Calcular a temperatura média de T1 e criar um segundo DataFrame com consumo acima de 70% do máximo **e** temperatura acima da média.
- Comparar os dois DataFrames e explicar o efeito da inclusão da temperatura como segundo critério.

## Todos os datasets da atividade (referência)

A atividade completa disponibiliza seis datasets do setor de energia; cada grupo resolve apenas o indicado pelo professor.

| # | Dataset | Link |
|---|---|---|
| 1 | Appliances Energy Prediction (UCI) | | https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction
| 2 | Steel Industry Energy Consumption (UCI) | | https://archive.ics.uci.edu/dataset/851/steel+industry+energy+consumption
| 3 | Power Consumption of Tetouan City (UCI) | | https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city
| 4 | Solar Power Generation Data (Kaggle) | | https://www.kaggle.com/datasets/anikannal/solar-power-generation-data
| 5 | Wind & Solar Energy Production (Kaggle) | | https://www.kaggle.com/datasets/henriupton/wind-solar-electricity-production
| 6 | Individual Household Electric Power Consumption (UCI) | | https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption
