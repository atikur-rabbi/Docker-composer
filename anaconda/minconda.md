```
sudo docker search continuumio
```

```
sudo docker pull continuumio/miniconda
```

```
sudo docker run -t -i continuumio/miniconda /bin/bash
```

```
conda info
```

```
sudo docker run -i -t -p 8888:8888 continuumio/miniconda /bin/bash
-c "/opt/conda/bin/conda install jupyter -y --quiet && mkdir
/opt/notebooks && /opt/conda/bin/jupyter notebook
--notebook-dir=/opt/notebooks --ip='*' --port=8888
--no-browser"
```

