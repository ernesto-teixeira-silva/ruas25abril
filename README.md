Este projeto foi desenvolvido no âmbito do desafio da Data Science for Social Good Portugal 3ª edição do #PlottingGoodDSSG (https://github.com/dssgPT/Plotting-Good-DSSG/tree/main/desafios/003_Liberdade_OSM)

## Organização das pastas/ficheiros

As pastas e ficheiros deste projeto encontra-se organizadas(os) no seguinte modo:

* dados_osm - Pasta com os ficheiros Open Street Map
    * portugal-latest-free.shp
        - **Fonte:** https://download.geofabrik.de/europe/portugal.html
    * concelhos-shapefile
        - **Fonte:** https://dados.gov.pt/pt/datasets/concelhos-de-portugal/
    * Cont_AAD_CAOP2021
        - **Fonte:** http://mapas.dgterritorio.pt/ATOM-download/CAOP-Cont/2021/Cont_AAD_CAOP2021.zip

* dssg_pt - Elementos da dssg pt referente ao desafio
        - **Fonte:** https://github.com/dssgPT/Plotting-Good-DSSG/tree/main/desafios/003_Liberdade_OSM

* notebook - Pasta com os notebooks referente ao desafio
    * desafio.ipynb - notebook de suporte à visualização criada no âmbito do desafio da dssg pt
    * ruas_25abril_algarve.ipynb - replicação do notebook disponibilizado pela dssg pt e para skills training

    **Nota:** Os notebooks correram no VSCode

* outputs - Pasta com ficheiros gerados nos notebooks

* pacotes - Bibliotecas carregadas para importar

    **Nota:** Por forma a evitar conflitos na importação das bibliotecas, foi efetuado o carregamento dos pacotes para o local e posterior instalação, sendo importante seguir esta ordem. Foram carregados pacotes do python 3.9 (cp39) para 64bits (amd64)

    - pygeos
    - GDAL
    - pyproject
    - Fiona
    - Shapely
    - geopandas
    - rasterio
    - geopy
    
    **Fonte:** https://www.lfd.uci.edu/~gohlke/pythonlibs/


## Instalar o ambiente

Para instalar o ambiente com as dependências necessárias foram corridos os seguintes comandos (na diretoria deste projeto):

Na linha de comando:

- 1. Criar o ambiente: `conda create -n <nome_ambiente> python=3.9 -y`
- 2. Ativar o ambiente: `conda activate <nome_ambiente>`
- 3. Instalar as dependências
    - Instalação dos pacotes gravados no local
        Na linha de comando e na diretoria `pacotes` executar para todas as bibliotecas o comando `pip install <nome_ficheiro_na_diretoria_pacotes>`:
            - **IMPORTANTE:** Seguir a ordem mencionada acima
            - Ex: pip install pygeos-0.12.0-cp39-cp39-win_amd64.whl
            
    - Instalação de outros pacotes:
        Na linha de comando eexecutar `pip install <nome_biblioteca>`, de:
            - sklearn
            - simpledbf
            - folium
            
