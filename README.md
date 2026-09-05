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

## Datasets da atividade

A atividade disponibiliza seis datasets do setor de energia.

**1. Appliances Energy Prediction (UCI)**
Identificar períodos de consumo elevado de eletrodomésticos numa residência e relacionar com temperatura/umidade.
Link: https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction

**2. Steel Industry Energy Consumption (UCI)**
Achar consumo elevado numa indústria siderúrgica e relacionar com carga e fator de potência.
Link: https://archive.ics.uci.edu/dataset/851/steel+industry+energy+consumption

**3. Power Consumption of Tetouan City (UCI)**
Identificar qual das três zonas da cidade tem o maior pico de consumo e as condições ambientais nesses momentos.
Link: https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city

**4. Solar Power Generation Data (Kaggle)**
Localizar períodos de alta geração numa usina fotovoltaica e quais inversores aparecem mais nesses momentos.
Link: https://www.kaggle.com/datasets/anikannal/solar-power-generation-data

**5. Wind & Solar Energy Production (Kaggle)**
Comparar picos de produção solar e eólica, cada uma avaliada contra sua própria escala.
Link: https://www.kaggle.com/datasets/ahmeduzaki/wind-and-solar-energy-production-dataset

**6. Individual Household Electric Power Consumption (UCI)**
Identificar demanda elétrica elevada com corrente acima da média numa residência; único dataset que exige tratamento de valores ausentes antes da amostragem.
Link: https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption

## Desafio Final — Análise de Dados de Energia com API Pública
 
**Problema:** uma equipe de planejamento energético precisa analisar o comportamento da carga elétrica de uma região atendida pelo Sistema Interligado Nacional (SIN), a partir de dados obtidos diretamente da API pública de Carga Verificada do ONS (Operador Nacional do Sistema Elétrico). No caso deste notebook, a análise cobre a área SP no período de 01/08/2025 a 07/08/2025.
 
**Solução:** a partir do JSON retornado pela API, o grupo constrói e inspeciona um DataFrame, organiza e trata os atributos (data/hora, área e valor de carga), calcula indicadores estatísticos (mínimo, máximo, média, mediana, amplitude), isola períodos de alta demanda (carga acima de 90% do pico) e aplica um segundo critério de recorte definido pela equipe (carga acima da média), comparando os dois grupos. A análise é fechada com dois gráficos (série temporal da carga e distribuição dos valores), uma síntese numérica dos resultados e um relatório técnico apoiado por IA (Gemini), submetido a uma validação crítica da equipe antes da versão final.
