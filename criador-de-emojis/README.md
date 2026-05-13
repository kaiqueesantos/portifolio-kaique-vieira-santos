# Manipulador de Emojis e Playlist Digital 🎨🎶

Este projeto em Python demonstra o uso de dicionários aninhados, matrizes e manipulação de listas para criar representações visuais de emojis, processar frequências musicais e gerenciar coleções de imagens baseadas em pixels.

## 🚀 Funcionalidades

O script está dividido em três pilares principais de processamento de dados:

### 1. Renderização de Emojis em Grade 👾
* **Estrutura de Matriz:** Utiliza uma grade 5x5 de tuplas RGB para desenhar um "Smile".
* **Visualização:** Emprega a biblioteca `matplotlib` para converter dados numéricos (RGB) em uma imagem visualizável no console ou notebook.

### 2. Processamento de Biblioteca Musical (Transposição) 🎵
* **Manipulação de Frequências:** Gerencia um dicionário de "Toques" musicais (Alegre e Triste).
* **Algoritmo de Transposição:** Percorre as matrizes de som e realiza a inversão de eixos (transposição), atualizando os valores originais no dicionário através do método `.update()`.

### 3. Gestão de Playlist de Imagens 🖼️
* **CRUD de Imagens:** Simula um sistema de gerenciamento de arquivos visuais.
* **Inserção Dinâmica:** Adiciona novos elementos (como a imagem "Fogo") em posições específicas da lista usando `.insert()`.
* **Remoção Logística:** Utiliza `.pop()` para remover o último item da coleção.
* **Iteração Profunda:** Varre chaves e valores para exibir detalhadamente os títulos das imagens e seus respectivos valores de pixels.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Biblioteca de Plotagem:** `matplotlib`
* **Conceitos de Programação:** * Dicionários aninhados (`dict`)
    * Matrizes e Tuplas
    * Loops aninhados (`for`)
    * Métodos de lista (`insert`, `pop`, `items`, `keys`)
    * Transposição de dados

## 📋 Exemplo de Estrutura de Dados

O projeto utiliza o seguinte formato para representar imagens em baixa resolução:
```python
{
  "titulo": "Sol",
  "pixels": (
    (255, 200, 0),
    (255, 220, 50),
    (200, 150, 0)
  )
}

pip install matplotlib

python criador_de_emojis.py
