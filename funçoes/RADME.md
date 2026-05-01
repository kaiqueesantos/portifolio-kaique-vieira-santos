# Coleção de Utilitários em Python (Funções Lógicas) 🛠️

Este repositório contém um conjunto de funções desenvolvidas em Python para automatizar cálculos comuns, desde a gestão de compras e análise climática até o acompanhamento acadêmico e financeiro.

## 📋 Funcionalidades do Projeto

O arquivo `funçoes.py` agrupa quatro sistemas principais, cada um focado em uma lógica de negócio específica:

### 1. Processador de Vendas com Desconto Progressivo 🛒
Calcula o valor total de uma compra baseada em múltiplos produtos e aplica descontos automáticos:
* **Regra de Desconto:** 10% para compras acima de R$ 500,00 e 5% para compras acima de R$ 200,00.
* **Validação:** Ignora itens com preços ou quantidades inválidas (zero ou negativas).

### 2. Analisador de Clima Semanal 🌡️
Monitora as variações de temperatura ao longo de uma semana (7 dias):
* **Estatísticas:** Calcula a média térmica semanal e conta quantos dias ultrapassaram os 35°C.
* **Alertas de Segurança:** Identifica temperaturas extremas (acima de 45°C ou abaixo de -5°C) e emite avisos de perigo.

### 3. Sistema de Gestão de Notas Acadêmicas 🎓
Automatiza a verificação de desempenho para turmas inteiras:
* **Critérios de Aprovação:** * Média ≥ 7.0: **Aprovado**
    * Média entre 5.0 e 6.9: **Recuperação**
    * Média < 5.0: **Reprovado**

### 4. Simulador de Poupança com Aportes Mensais 💰
Projeta o crescimento de patrimônio considerando juros compostos e depósitos variáveis:
* **Dinâmica:** O usuário define uma taxa mensal e pode realizar novos depósitos a cada mês.
* **Meta de Investimento:** O sistema sinaliza automaticamente quando o saldo ultrapassa a marca de R$ 10.000,00.

## 🛠️ Conceitos de Programação Aplicados

Este projeto demonstra o uso prático de:
* **Estruturas de Repetição:** `for i in range()` para processamento de listas de dados e tempo (meses/dias).
* **Estruturas Condicionais:** `if/elif/else` para tomada de decisão e aplicação de regras de negócio.
* **Manipulação de Tipos:** Conversão de entradas de usuário (`input`) para `float` e `int`.
* **Formatação de Dados:** Uso de `round()` para precisão monetária e térmica.

## 🚀 Como Utilizar

1.  Certifique-se de ter o Python 3 instalado.
2.  Importe as funções ou execute o arquivo diretamente.
3.  Para iniciar qualquer sistema, chame a função desejada no console:
    ```python
    processar_vendas()
    analisar_clima()
    sistema_notas_turma()
    simulador_poupanca()
    ```

---
*Desenvolvido como um exercício de lógica de programação e automação de processos.*
