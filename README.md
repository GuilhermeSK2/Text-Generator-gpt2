# Gerador de Texto em Português com GPT-2

Este projeto demonstra a utilização de um modelo de linguagem pré-treinado, o GPT-2 em português (`pierreguillou/gpt2-small-portuguese`), para gerar texto a partir de um prompt inicial. A implementação é feita usando a biblioteca `transformers` da Hugging Face, que facilita o uso de modelos de linguagem de última geração.

## Visão Geral

Modelos de linguagem como o GPT-2 são redes neurais complexas treinadas em vastas quantidades de texto para aprender padrões de linguagem. Uma vez treinados, eles podem gerar texto que imita o estilo e o conteúdo dos dados em que foram treinados. Este projeto foca na geração de texto em português, explorando a capacidade do modelo de criar continuidades a partir de frases fornecidas.

## Estrutura do Projeto

* `TextGenerator.ipynb`: O notebook Jupyter que contém todo o código para configurar o ambiente, carregar o modelo e gerar texto.

## Tecnologias Utilizadas

* **Python 3**
* **Hugging Face `transformers` library**: Para acesso e utilização do modelo GPT-2.
* **Jupyter Notebook**: Para execução e demonstração interativa do código.
* **Modelo**: `pierreguillou/gpt2-small-portuguese` (um modelo GPT-2 pequeno adaptado para o português).

## Exemplo de Uso

No notebook, você pode modificar a variável `text` para experimentar diferentes prompts e ver como o modelo gera texto a partir deles. O parâmetro `max_length` controla o tamanho máximo do texto gerado, e `do_sample=True` permite uma geração mais criativa e menos determinística.

```python
text = "A inteligência artificial está transformando o mundo"
resultado = gerador(text, max_length=150, do_sample=True, temperature=0.7)
print(resultado)
