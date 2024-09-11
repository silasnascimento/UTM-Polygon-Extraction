# UTM-Polygon-Extraction
Script para extração de coordenadas UTM de PDFs e criação de poligonais em GeoPackage

# Extração de Coordenadas UTM e Criação de Poligonal para Memorial Descritivo

Este repositório contém um notebook em Python que automatiza a extração de coordenadas UTM a partir de um documento PDF e gera uma poligonal utilizando bibliotecas de geoprocessamento como Shapely e GeoPandas. A solução foi desenvolvida para otimizar a criação de poligonais de memoriais descritivos no formato necessário para sistemas GIS.

# Funcionalidades

Extração de coordenadas UTM: O script lê documentos PDF e utiliza expressões regulares (módulo re) para identificar e extrair coordenadas no formato "N 7.747.897,01 m. e E 684.187,64 m.".
Criação de poligonais: Após a extração das coordenadas, o script utiliza o Shapely para gerar poligonais.
Exportação para Geodatabase: O polígono gerado é exportado para um arquivo GeoPackage (GPKG) usando GeoPandas, pronto para ser integrado em qualquer software GIS.

# Estrutura do Projeto
PDF_to_feature.ipynb: O notebook que contém o código completo para extração de coordenadas, criação de poligonal e exportação para GeoPackage.
Exemplo de entrada: Um arquivo PDF contendo coordenadas UTM no formato textual.
Exemplo de saída: Um GeoPackage contendo a poligonal criada a partir das coordenadas extraídas.

# Como Usar
Clone este repositório:

bash
código
git clone https://github.com/seu-usuario/UTM-Polygon-Extraction.git
Instale as dependências necessárias:

bash
código
pip install -r requirements.txt
Execute o notebook PDF_to_feature.ipynb em um ambiente Jupyter ou JupyterLab. Certifique-se de ter um arquivo PDF no formato esperado.

No notebook, defina os caminhos corretos para o arquivo PDF de entrada e o caminho de saída para o GeoPackage.

Execute as células do notebook para gerar a poligonal e exportar o resultado.

# Requisitos

Python 3.7+
Bibliotecas:
PyPDF2
GeoPandas
Shapely
re (incluso no Python)

