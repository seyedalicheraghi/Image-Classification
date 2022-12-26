# Image-Classification
## API


`onnx_model`: ONNX model to convert

`input_names`: list with graph input names

`input_shapes`: override input shapes (experimental)

`verbose`: detailed output

## Getting started
### Conda (Recommended)

Create a conda environment called tfe with all dependencies. 

```commandline ```

conda env create -f tfe.yml

conda activate tfe

python -m ipykernel install --name=tfe

### Install requried libraries in your system following "Install Required Libraries.ipynb" instructions.

#### What are the purposes of this Repo:
* Step 1: Develope and train a very basic and simple classification model to differentiate between John Wick vs Rambo photos using "Training.ipynb" scripts.

![alt text](model.png)

* Step 2: Convert the model I trained in previous step into two formats: ONNX and Keras using "Training.ipynb" scripts.

* Step 3: Evaluate the ONNX model to check if we loose accuracy in conversion step using "ONNX Evaluation.ipynb" scripts.

* Step 4: Convert the ONNX model into TensorRT Engine using Google Colab and Inference the TRT model using "Convert ONNX to TRT.ipynb" scripts.

After producing the ONNX model in step 2 and evaluating it in step 3, you need to copy the model into the google colab.

Based on the model we evaluate, we can choose different form of accuracy measurement. 

Precisin and Recall are good factors to evalaute a classification model.

mAP is usually used to measure the performance of a Detection Model.

To measure the inference speed we can either load images from a testing directory and 

