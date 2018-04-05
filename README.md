# Desafio de Programação

Trata-se de um teste simples para avaliação de competências técnicas necessárias para o desenvolvimento de rotinas ETL utilizando Python como base.

## Problema

Possuímos arquivos de texto contendo uma lista de coordenadas geográficas obtidas a partir do GPS de dispositivos móveis. Precisamos que esses arquivos sejam processados e enriquecidos com informações disponíveis na internet. O objetivo do enriquecimento é descobrir os endereços correspondentes às coordenadas. Para essa finalidade deve ser utilizada alguma API aberta, como por exemplo: _Google Maps_.

## Requisitos

1. A solução deve ser implementada em Python;
2. A solução como um todo deve poder ser executada em ambiente Linux;
3. Todas as bibliotecas, produtos ou serviços utilizados devem ser open source;
4. As configurações de conexão com banco de dados devem ser parametrizadas;
5. Caso necessário, um script DDL deve ser fornecido e devidamente documentado;

## Insumos

Os dados necessários para o desenvolvimento da solução estão disponíveis através do link
[data_points](https://s3.amazonaws.com/dev.etl.python/datasets/data_points.tar.gz).

O arquivo consiste de uma série de coordenadas geográficas compostas por:

- Latitude
- Longitude
- Distância

**OBS: Em todas as linhas, os três atributos são apresentados em dois formatos:**

- Em graus, minutos e segundos
- Em número decimal

Exemplo:

> Latitude: 30°02′59″S   -30.04982864  
> Longitude: 51°12′05″W   -51.20150245  
> Distance: 2.2959 km  Bearing: 137.352°  

## Resultados

O dataframe final deve ser salvo em um banco de dados relacional e precisa conter as seguintes informações:

latitude|longitude|rua|numero|bairro|cidade|cep|estado|pais|endereço completo
--------|---------|---|------|------|------|---|------|----|-----------------

Os seguintes quesitos serão avaliados:

- Estratégia de implementação
- Clareza do código
- Testes e validações
- Eficiência da implementação
- Documentação

## Bônus

Além do enriquecimento proposto, que análises poderiam ser feitas utilizando essa massa de dados? Que métricas poderiam ser obtidas?
