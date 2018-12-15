# Yolo3-voc-train
### Dataset
VOC2007
### Dependences
The code has been tested in python 3.6, ubuntu 16.04.
1. keras-gpu
2. tensorflow-gpu
3. matplotlib
4. Pillow
5. opencv

### Run with GPU:
conda create -n yolo3 python=3.6 keras-gpu tensorflow-gpu matplotlib

activate yolo3

pip install Pillow

wget https://pjreddie.com/media/files/yolov3.weights

python convert.py -w yolov3.cfg yolov3.weights model_data/yolo_weights.h5

python train.py

conda install nb_conda_kernels

python -m ipykernel install --user --name yolo3 --display-name "Yolo3"
