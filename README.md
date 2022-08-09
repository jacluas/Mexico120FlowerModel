# Mexico 120 Flower Model
### Pre-trained 512-VGG model (from Mexico 120 Flower dataset)

We share the pre-trained 512-VGG CNN model as research support in Mexico native flora identification. We believe that this pre-trained model may be a good starting point for future research in flower identification. Transfer learning from pre-trained models on ImageNet 2012 dataset was used.

### Usage

The model is shared in the form of H5 format, that is, a file format to store structured data to easily share. Keras saves models in this format as it can easily store the weights and model configuration in a single file. We used Keras version 2.2.4, with Tensorflow 1.13.1 as backend, and Python version 3.7.3.

### How to consume the pre-trained 512-VGG model (from Mexico 120 Flower dataset)

We used Keras version 2.2.4, with Tensorflow 1.13.1 as backend, and Python version 3.7.3.


```python
python predict.py MODEL_NAME.h5 IMAGE_TEST_PATCH
```

Examples:
```python
	python predict.py model_512_vgg TEST/Achillea_millefolium/p_1.png
	python predict.py model_512_vgg TEST/Cordia_boissieri/GBN_2.png
	python predict.py model_512_vgg TEST/Ipomoea_triloba/GBN_1.png
```
