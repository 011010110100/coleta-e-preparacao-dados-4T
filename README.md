# Projeto de Coleta e Preparação de Dados - Fase 1

Este repositório contém o código e os dados da primeira fase do projeto de coleta e preparação de dados. O objetivo principal desta fase é criar um conjunto de dados consolidado em formato CSV, combinando informações de países obtidas de uma API REST e dados de Produto Interno Bruto (PIB) obtidos de um arquivo CSV.

## Objetivos

* Coletar dados de países (código, nome, moeda, população, capital, área e continente) de uma API REST local.
* Ler dados de PIB de um arquivo CSV, contendo informações de 1960 a 2021.
* Combinar os dados das duas fontes em um único DataFrame Pandas.
* Limpar e transformar os dados, tratando valores ausentes e inconsistências.
* Salvar o DataFrame resultante em um arquivo CSV, com uma linha por país e colunas para cada ano de PIB.
* Documentar o processo de coleta e preparação de dados em notebooks Jupyter.

## Arquivos

* `api_fase01.py`: Código da API REST local que fornece dados de países.
* `country.json`: Arquivo JSON com informações adicionais sobre os países.
* `gpd_data.csv`: Arquivo CSV com dados de PIB dos países.
* `README.md`: Este arquivo, explicando o projeto.
* `fase1.csv`: arquivo contendo o arquivo CSV final com os dados consolidados.

## Como executar

1.  Clone este repositório para sua máquina local.
2.  Siga as instruções no arquivo `README.md` fornecido no arquivo zipado para configurar e iniciar a API REST local.
3.  Certifique-se de ter o Python 3 e as bibliotecas Pandas, Requests, Flask e Flask-RESTful instaladas.
4.  Execute os notebooks Jupyter na pasta `notebooks/` para coletar, preparar e consolidar os dados.
5.  O arquivo CSV final será gerado como 'fase1.csv'.

## Dependências

* Python 3
* Pandas
* Requests
* Flask
* Flask-RESTful

## Sugestão para criar o ambiente virtual (WSL)

Criando o ambiente
>> python -m venv fase1CPD
            
Ativando ambiente virtual
>> source fase1CPD/bin/activate
            
Instalando as demais dependências.
>> pip install -r ./requirements.txt

Inicializando a API
>> python api_fase01.py

## Autor

\[Marcos de Brito Paceka]

## Licença

Este projeto está licenciado sob a [Licença MIT] - veja o arquivo [LICENSE.md] para detalhes. (opcional)
