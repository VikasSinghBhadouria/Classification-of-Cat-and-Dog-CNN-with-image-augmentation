# Classification-of-Cat-and-Dog using CNN with image augmentation
Classification of  images between two class cat and dog  using CNN with image augmentation .

We are using image augmentation to increase the amount of training data using augmentation by 
using from keras.preprocessing.image import ImageDataGenerator.

Data is very limited and costly in some cases such as medical imagery.
To get the best out of it , we are using ImageDataGenerator and creating multiple images  for each image we have in our training data set by rotation ,zoon in , shearing , tilting ,rescaling.

fill_mode for method used to  decide the color of newly generated pixel in case of shear n zoom in. 

datagen = ImageDataGenerator(
        rotation_range=40,
        width_shift_range=0.2,
        height_shift_range=0.2,
        rescale=1./255,
        shear_range=0.2,
        zoom_range=0.2,
        horizontal_flip=True,
        fill_mode='nearest')
  
For details , read Documentation :http://keras.io/preprocessing/image/

It uses data that can be downloaded at:
https://www.kaggle.com/c/dogs-vs-cats/data
In our setup, we:
- created a data/ folder
- created train/ and validation/ subfolders inside data/
- created cats/ and dogs/ subfolders inside train/ and validation/
We are using mini-data  as that will be enough for our purpose .
So that we have 1000 training examples for each class, and 450 validation examples for both class.
In summary, this is our directory structure:
```
data/
    train/
        dogs/
            dog001.jpg
            dog002.jpg
            ...
        cats/
            cat001.jpg
            cat002.jpg
            ...
    validation/
        dogs/
            dog001.jpg
            dog002.jpg
            ...
        cats/
            cat001.jpg
            cat002.jpg
            ...
```
'''




Reference : https://gist.github.com/fchollet/0830affa1f7f19fd47b06d4cf89ed44d
