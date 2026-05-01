# Analisador de Vendas e Segurança 📊

Este projeto consiste em um script Python desenvolvido para analisar um conjunto de vendas, calcular médias e aplicar regras de segurança para identificar possíveis anomalias ou necessidades de revisão manual.

## ✨ Funcionalidades

O script realiza as seguintes operações:

1.  **Entrada de Dados:** Solicita ao usuário os valores de três vendas distintas.
2.  **Processamento de Média:** Calcula a média aritmética simples das vendas informadas.
3.  **Gestão de Configuração:** Exibe e permite a alteração dinâmica de um `LIMITE_SEGURANCA` global durante a execução.
4.  **Verificações de Segurança:**
    *   **Quarentena:** Ativa um alerta caso a média das vendas ultrapasse o limite de segurança definido.
    *   **Revisão Manual:** Ativa um alerta caso qualquer uma das vendas individuais seja 5 vezes superior à média calculada (identificação de *outliers*).

## 🛠️ Tecnologias Utilizadas

*   **Linguagem:** Python 3
*   **Conceitos Aplicados:** Funções, escopo global (`global`), casting de tipos (`float`), estruturas condicionais e entrada/saída de dados.

## 🚀 Como Executar

1.  Certifique-se de ter o Python instalado em sua máquina.
2.  Copie o código do arquivo para um arquivo local (ex: `analisador.py`).
3.  Execute o script via terminal:
    ```bash
    python analisador.py
    ```
4.  Siga as instruções na tela para inserir os valores das vendas e decidir sobre a alteração do limite de segurança.

## 📝 Exemplo de Regras de Negócio

*   **Limite Padrão:** R$ 10.000,00.
*   **Alerta de Quarentena:** Disparado se `Média > Limite`.
*   **Alerta de Revisão:** Disparado se `Venda_X > (Média * 5)`.

---
*Projeto desenvolvido para fins de estudo de lógica de programação e manipulação de variáveis em Python.*
