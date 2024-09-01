# Sobre o trabalho
Este trabalho trata-se de um exercício programa (EP) da  disciplina MAC5921 - Deep Learning do programa de pós-graduação em Ciência da Computação do IME-USP. A proposta desse trabalho consiste em comparar o desempenho de redes neurais convolucionais e redes neurais fully connected simples para a classificação de imagens.

O conjunto de dados utilizado para este trabalho é o [Kuzushiji-MNIST](https://github.com/rois-codh/kmnist), no qual esse repositório é um fork do repositório original que contém mais informações sobre o cunjunto de dados. Nesse repositório há a possibilidade de download de 3 datasets (Kuzushiji-MNIST, Kuzushiji-49 e Kuzushiji-Kanji), o escolhido para esse trabalho foi o Kuzushiji-MNIST dado ser o conjunto com a menor quantidade de classes, o que facilita os experimentos. 

# Modelos treinados




# Resultados



# Instruções

## Configurar ambiente


Para realizar os experimentos, foi utilizado um ambiente virtual do conda utilizando o python 3.10.12. O ambiente pode ser criado como abaixo:

```
conda create --name env-kmnist  python=3.10.12
```

Para instalar os pacotes utilizados para os experiementos, dentro do ambiente virtual do conda, utilize o comando abaixo:

```
pip install -r requirements
```

## Download do dataset

Para realizar o download do dataset, rode o comando:

```
python src/download_data.py
```

Dessa forma o dataset irá ser baixado e colocado na pasta data/

## Experimentos

Para reproduzir os experimentos basta rodar o notebook `notebooks/classification.ipynb` para treinar e testar os modelos. Assim, os melhores modelos serão salvos no diretório `models`, os logs do treinamento dos modelos irão constar no diretório `logs` e os resultados dos modelos no conjunto de treino e de teste irão estar no diretório `results`.




