# Iris 👁 Detection with TensorFlow

In this project I created a `TensorFlow` model which can track eyes and project dots on my eyes 👀 as I move my to and away from the screen.

The model uses a pretrained `ResNet` model and I add more layers on top to train the model to track my eyes. I use images annotated with the point locations of my eye on a image. The annotation of images is done using `LabelMe` library in python and then the data is augmented using `albumentations` library.

# Running the Notebook ❓

Just create a new environment in `anaconda` or `vnev` and activate the environment and use the following command to install all the dependencies:

```Bash
pip install -r requirements.txt
```

### ⚠ Only train the model locally, if you have a good Nvidia GPU. **DO NOT** train on CPU, each epoch will take atleast 2 hours to train and the model needs to atleast train for 10 epochs to perform reasonably well. So, if you do not have a Nvidia GPU, train on Google Colab Notebooks.

#### And there you have it, the model is trained to detect eyes in real-time using `Tensorflow` and `OpenCV` ✅ 🏁.