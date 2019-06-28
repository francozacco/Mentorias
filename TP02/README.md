* Para correr el notebook con Docker
    - Opcion 1
    docker run -it --rm -p 8888:8888 -v $PWD/dataset:/home/jovyan/dataset -v $PWD/TP02.ipynb:/home/jovyan/TP02.ipynb -e NB_UID=`id -u` francopaludi2/diplodatos2019:dscience
    Copiar URL en browser y correr el notebook

    - Opcion 2 (más lenta)
    docker build -f Dockerfile -t dscience .
    docker run -it --rm -p 8888:8888 -v $PWD/dataset:/home/jovyan/dataset -v $PWD/TP02.ipynb:/home/jovyan/TP02.ipynb -e NB_UID=`id -u` dscience:latest
    Copiar URL en browser y correr el notebook

