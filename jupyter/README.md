Jupyter Scipy

```
docker run -p 8888:8888 jupyter/scipy-notebook:17aba6048f44
```

Anaconda

```
docker run -i -t -p 8888:8888 continuumio/anaconda3 /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet && mkdir /opt/notebooks && /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser" --allow-root 
```

--allow-root 

```
docker run -i -t -p 8888:8888 continuumio/anaconda /bin/bash


docker run -i -t -p 8888:8888 continuumio/anaconda3 /bin/bash
```

