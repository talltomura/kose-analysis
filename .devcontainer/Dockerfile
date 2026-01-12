#Base
FROM jupyter/datascience-notebook:python-3.11

#For GPU
#FROM jupyter/datascience-notebook:cuda12-python-3.11

#aptget

#conda-forge
RUN conda install -y -c conda-forge \
    geopandas \
    osmnx \
    rasterio \
 && conda clean -afy

#Attachements
COPY requirements.txt /tmp/requirements.txt
RUN pip install --no-cache-dir -r /tmp/requirements.txt
