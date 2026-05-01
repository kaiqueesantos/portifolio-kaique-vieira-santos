# Análise de Microclima e Simulador de Evacuação 🏢🌡️

Este projeto em Python está dividido em duas frentes de estudo: a análise da qualidade do ar e conforto térmico em pontos estratégicos de São Paulo, e uma simulação lógica de evacuação baseada em um cenário real (1º andar da UNICID).

---

## 🌤️ Parte 1: Análise de Microclima Urbano

Este módulo processa dados de sensores (baseados em fontes como CETESB e Climatempo) coletados em diferentes horários do dia para calcular o bem-estar do cidadão.

### Funcionalidades
* **Processamento de Dados:** Analisa Nome do local, Horário, Temperatura, Umidade e IQA (Índice de Qualidade do Ar).
* **Classificação IQA:** Categoriza a qualidade do ar entre "Boa" e "Péssima" seguindo as faixas oficiais.
* **Cálculo de Nota de Conforto:**
    * **Temperatura:** Ideal entre 20°C e 26°C.
    * **Umidade:** Ideal entre 50% e 70%.
    * **Pesos:** A nota final (0 a 10) é composta por Temperatura (40%), Umidade (30%) e IQA (30%).
* **Veredicto:** Sugere se o ambiente está propício para caminhadas ou se oferece riscos a grupos sensíveis (asmáticos/riniticos).

---

## 🏃 Parte 2: Simulador de Evacuação (UNICID)

Um algoritmo de tomada de decisão que simula um agente tentando sair do fundo do 1º andar até a Rua Cesário Galeno.

### Dinâmica do Simulação
* **Sistema de Energia:** O agente inicia com 18 pontos de energia; cada ação ou movimento consome uma quantidade específica de fôlego.
* **Gestão de Inventário:** O agente pode coletar itens como extintores e crachás de emergência para superar obstáculos.
* **Interação com o Cenário:**
    * **Bloqueios:** Cadeiras no caminho exigem esforço físico extra.
    * **Segurança:** Portas magnéticas exigem crachá ou o uso de força bruta (gasto alto de energia com extintor).
    * **Perigos:** Áreas com fumaça exigem estratégia (uso de extintor ou agachar para passar).
* **Objetivo:** Chegar ao ponto final da lista de locais antes que a energia chegue a zero.

---

## 🛠️ Tecnologias e Conceitos Utilizados

* **Linguagem:** Python 3.10+
* **Estruturas de Dados:** Listas aninhadas e listas simples.
* **Lógica de Controle:** * Loops `for` para processamento de dados em lote.
    * Loops `while` para simulações baseadas em estados.
    * Estrutura `match/case` para classificações complexas.
* **Matemática Básica:** Cálculos de média ponderada e arredondamentos.

---

## 🚀 Como Executar

1.  Certifique-se de ter o Python instalado.
2.  Execute o arquivo:
    ```bash
    python conceitos_de_lista.py
    ```
3.  O resultado da análise climática e o log passo a passo da evacuação serão exibidos no console.
