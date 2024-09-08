# Sobre o trabalho

Este trabalho trata-se de um exercício programa (EP) da  disciplina MAC5921 - Deep Learning do programa de pós-graduação em Ciência da Computação do IME-USP. A proposta desse trabalho consiste em comparar o desempenho de redes neurais convolucionais e redes neurais fully connected simples para a classificação de imagens.

O conjunto de dados utilizado para este trabalho é o [Kuzushiji-MNIST](https://github.com/rois-codh/kmnist). Nesse repositório há a possibilidade de download de 3 datasets (Kuzushiji-MNIST, Kuzushiji-49 e Kuzushiji-Kanji), o escolhido para esse trabalho foi o Kuzushiji-MNIST dado ser o conjunto com a menor quantidade de classes, o que facilita os experimentos. 

O Kuzushiji-MNIST possui um total de 10 classes, sendo cada uma delas um caracter do Hiragana. Uma representação de cada uma das classes pode ser vista abaixo, sendo cada "linha" uma classe, a primeira "coluna" sendo um bom exemplo (digital) do caracter e as outras sendo exemplos escritos à mão.

<p align="center">
  <img src="images/kmnist_examples.png" />
</p>

# Resultados obtidos

Os resultados obtidos podem ser vistos no relatório que está no arquivo `relatorio/relatorio.pdf`.

# Instruções de execução

## 1. Configurar ambiente


Para realizar os experimentos, foi utilizado um ambiente virtual do conda utilizando o python 3.10.12. O ambiente pode ser criado como abaixo:

```
conda create --name env-kmnist  python=3.10.12
```

Para instalar os pacotes utilizados para os experiementos, dentro do ambiente virtual do conda, utilize o comando abaixo:

```
pip install -r requirements
```

## 2. Download do dataset

Para realizar o download do dataset, rode o comando:

```
python src/download_data.py
```

Dessa forma o dataset irá ser baixado e colocado na pasta `data/`

## 3. Reproduzir experimentos

Para reproduzir os experimentos basta executar o notebook `notebooks/1.classification.ipynb` para treinar e testar os modelos. Assim, os melhores modelos serão salvos no diretório `models`, os logs do treinamento dos modelos irão constar no diretório `logs` e os resultados dos modelos no conjunto de treino e de teste irão estar no diretório `results`.

Após reproduzir os gráficos e tabelas com os resultados, é possível através do notebook `notebooks/2.results_analysis.ipynb` gerar os gráficos de desempenho do modelo no treinamento, que estarão no diretório `images/results_plt/`, e também gerar as tabelas de com as métricas de classificação (acurácia, recall, precision, F1, etc) que estarão no diretório `results/metrics/`.

Para obter as imagens das arquiteturas dos modelos e dos kernels, rode o notebook `notebooks/3.models_analysis.ipynb`. Para gerar a imagem da arquitetura do modelo, garanta que tem instalado em seu ambiente o graphviz, instale com `sudo apt install graphviz -y`









