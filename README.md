
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


