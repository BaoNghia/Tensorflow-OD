# Tensorflow Object Detection

## Installation
First install requirement.txt
'''
pip install -r requirement.txt
'''

Then, install Tensorflow API
'''
git clone https://github.com/tensorflow/models.git

cd models/research
# Compile protos.
protoc object_detection/protos/*.proto --python_out=.
# Install TensorFlow Object Detection API.
cp object_detection/packages/tf2/setup.py .
python -m pip install .

# Test the installation.
python object_detection/builders/model_builder_tf2_test.py
'''
