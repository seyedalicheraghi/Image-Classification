# Image-Classification
## API


`onnx_model`: ONNX model to convert

`input_names`: list with graph input names

`input_shapes`: override input shapes (experimental)

`verbose`: detailed output

`change_ordering:` change ordering to HWC (experimental)
## Getting started
### Conda (Recommended)

Create a conda environment called tf with all dependencies. This command prepare the environment for Flex-Logix scripts. 
```commandline
conda env create -tf.yml
conda activate tf

python -m ipykernel install --name=tf

### Install requried libraries in your system following "Install Required Libraries.ipynb" instructions.
#### What are the purposes of this Repo:
* Step 1: Develope and train a very basic and simple classification model to differentiate between John Wick vs Rambo photos using "Training.ipynb" scripts.
* Step 2: Convert the model I trained in previous step into two formats: ONNX and Keras using "Training.ipynb" scripts.
* Step 3: Evaluate the ONNX model to check if we loose accuracy in conversion step using "ONNX Evaluation.ipynb" scripts.
* Step 4: Convert the ONNX model into TensorRT Engine using Google Colab using "Convert ONNX to TRT.ipynb" scripts.
* Step 5: Evaluate the TensorRT engine model to check if we loose accuracy in conversion step using "TRT Inference.ipynb" scripts.


