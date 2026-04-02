# Apresentação - Algoritmo KNN

Esta pasta contém os arquivos necessários para gerar a apresentação baseada na implementação do algoritmo KNN.

Como a apresentação é feita em [Quarto](https://quarto.org/) e possui blocos de código em Python executados dinamicamente para gerar os gráficos dos slides, é necessário instalar algumas dependências.

## Pré-requisitos

1. Ter o **Quarto CLI** instalado.
2. Ter o **Python 3** instalado.

## Instalação das bibliotecas

Para instalar os pacotes do Jupyter e as bibliotecas de Data Science (Scikit-Learn, Matplotlib, etc.) exigidas, abra o terminal nesta pasta e execute:

```bash
pip install -r requirements.txt
```

*(Se o seu sistema usa `python3` por padrão e der algum erro, você pode usar: `python3 -m pip install -r requirements.txt`)*

## Renderizando a apresentação

Para gerar o HTML final para visualização estática:
```bash
quarto render presentation.qmd
```

Para visualizar a apresentação em tempo real em seu navegador (com recarregamento automático a cada alteração salva):
```bash
quarto preview presentation.qmd
```