#Base
FROM jupyter/datascience-notebook:python-3.11

#For GPU
#FROM jupyter/datascience-notebook:cuda12-python-3.11

#aptget

#conda-forge
RUN conda install -y -c conda-forge \
    geopandas \
    mapclassify \ 
    rasterio \
    earthengine-api \
 && conda clean -afy

#Attachements
#If you need use pip install, list items on requirements.txt
COPY requirements.txt /tmp/requirements.txt
RUN pip install --no-cache-dir -r /tmp/requirements.txt
