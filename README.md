# CNN Image Classifier with Keras
Image classification with Keras using CNN architecture

## Getting started with local machine
```
pip install -r requirements.txt
# for GPU optimized computation
pip install -r requirements-gpu.txt


jupyter notebook image_classifier.ipynb
```

## Running on Cloud Computing
```
pip install -r requirements-gpu.txt


jupyter notebook --generate-config


sed -ie "s/#c.NotebookApp.ip = 'localhost'/#c.NotebookApp.ip = '*'/g" ~/.jupyter/jupyter_notebook_config.py


jupyter notebook --ip=0.0.0.0 --no-browser
```

## Load example images for traning and testing
This dataset contains 5 categories of fruits. This data was obtained from [Fruit-Images-Dataset](https://github.com/Horea94/Fruit-Images-Dataset) (original dataset has more fruits categories).
```
curl https://s3-ap-southeast-1.amazonaws.com/input-dataset/fruit_images.zip -o ~/images.zip

unzip ~/images.zip -d .

rm ~/images.zip
```
