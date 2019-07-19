# reference: https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html
FROM jupyter/scipy-notebook

# Add metadata
# version="1.0"
LABEL maintainer="Franco Paludi <francopaludi2@gmail.com>"

# Set environment variables
ENV LANG=C.UTF-8 LC_ALL=C.UTF-8

# Update useful packages
# RUN conda update -y 'ipywidgets' \
# 'pandas' \
# 'numexpr' \
# 'matplotlib' \
# 'scipy' \
# 'seaborn' \
# 'scikit-learn' \
# 'scikit-image' \
# 'sympy' \
# 'cython' \
# 'patsy' \
# 'statsmodels' \
# 'cloudpickle' \
# 'dill' \
# 'dask' \
# 'numba' \
# 'bokeh' \
# 'sqlalchemy' \
# 'hdf5' \
# 'h5py' \
# 'vincent' \
# 'beautifulsoup4' \
# 'protobuf' \
# 'xlrd'

RUN pip install astropy
RUN pip install plotly
RUN pip install cufflinks

# Add files related to the project
# ADD TP02.ipynb

# Entrypoint
#ENTRYPOINT start.sh jupyter nbconvert --execute --to notebook --output-dir=model --output=TP02.log TP02.ipynb
ENTRYPOINT start.sh jupyter-notebook TP02.ipynb



