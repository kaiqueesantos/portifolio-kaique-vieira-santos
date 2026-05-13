# Sistema de Auditoria de Recursos Corporativos 🏦🔍

Este projeto consiste em uma ferramenta robusta para análise orçamentária e auditoria de processos em estruturas empresariais hierárquicas. O sistema utiliza técnicas avançadas de programação funcional para percorrer departamentos, calcular custos e realizar conversões monetárias em tempo real.

## 🚀 Funcionalidades Principais

* **Cálculo Hierárquico Recursivo:** O sistema percorre uma estrutura de dados aninhada (dicionários dentro de dicionários) para somar orçamentos de subdepartamentos de forma automática.
* **Auditoria via Decorators:** Utiliza o padrão de projeto *Decorator* para monitorar a execução de funções, registrando o tempo de processamento, parâmetros utilizados e metadados da auditoria.
* **Filtros Dinâmicos (*Args):** Permite ignorar departamentos específicos durante o cálculo (ex: gerar um relatório excluindo os custos de "TI" ou "RH").
* **Conversão de Moeda (*Kwargs):** Suporte flexível para conversão de valores (BRL para USD, EUR, etc.) através de parâmetros nomeados dinâmicos.

## 🛠️ Tecnologias e Conceitos Aplicados

* **Linguagem:** Python 3.
* **Decoradores (@auditor):** Para separação de preocupações (*logging* e monitoramento).
* **Recursividade:** Algoritmo de soma que se adapta à profundidade da estrutura da empresa.
* **Argumentos Arbitrários:** Uso de `*args` para listas de exclusão e `**kwargs` para configurações de câmbio.
* **Biblioteca `time`:** Para medição de performance e eficiência do código.

## 📊 Estrutura de Exemplo

O sistema processa uma matriz organizacional detalhada, como no exemplo abaixo:
* **TI:** Infraestrutura (Servidores, Segurança) e Desenvolvimento (Frontend, Backend, DevOps).
* **RH:** Recrutamento, Treinamento e Cultura (Eventos, Brindes).
* **Financeiro:** Gestão direta de ativos.

## ⚙️ Como Utilizar

1.  **Execução do Script:**
    ```bash
    python sistema_de_auditoria_de_recursos_corporativos.py
    ```

2.  **Exemplos de Chamadas no Código:**
    * *Cálculo Total:* `calcular_orcamento(empresa_data)`
    * *Excluindo Departamentos:* `calcular_orcamento(empresa_data, "TI")`
    * *Conversão Internacional:* `calcular_orcamento(empresa_data, moeda_destino="USD", taxa_cambio=0.19)`

## 📝 Exemplo de Saída da Auditoria

```text
========== INICIO DA AUDITORIA ==========
Funcao chamada: calcular_orcamento
Departamentos ignorados: ('RH',)
Parametros de conversao: {'moeda_destino': 'EUR', 'taxa_cambio': 0.17}
...
Tempo de execucao: 0.00002 segundos
=========================================
