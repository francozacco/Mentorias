* Para correr el notebook con Docker
    docker build -f Dockerfile -t dscience .
    docker run -it --rm -p 8888:8888 -v $PWD/dataset:/home/jovyan/dataset -v $PWD/TP02.ipynb:/home/jovyan/TP02.ipynb -e NB_UID=`id -u` dscience:latest
    Copiar URL en browser y correr el notebook
