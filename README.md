# Multiple-object-tracking
### Environment
#### Python 3.6.7
#### Keras 2.2.4
#### Tensorflow 1.12.0

### Run with GPU:
conda create -n yolo3 python=3.6 keras-gpu tensorflow-gpu matplotlib

activate yolo3

pip install Pillow

wget https://pjreddie.com/media/files/yolov3.weights

python convert.py -w yolov3.cfg yolov3.weights model_data/yolo_weights.h5

python train.py

conda install nb_conda_kernels

python -m ipykernel install --user --name yolo3 --display-name "Yolo3"
