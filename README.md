# CNN Image Classifier with Keras
Image classification with Keras using CNN architecture

## Getting started with local machine
```
pip install -r requirements.txt
# for GPU optimized computation
pip install -r requitements-gpu.txt


jupyter notebook image_classifier.ipynb
```

## Running on Cloud Computing
```
pip install -r requirements-gpu.txt


jupyter notebook --generate-config


sed -ie "s/#c.NotebookApp.ip = 'localhost'/#c.NotebookApp.ip = '*'/g" ~/.jupyter/jupyter_notebook_config.py


jupyter notebook --ip=0.0.0.0 --no-browser
```
