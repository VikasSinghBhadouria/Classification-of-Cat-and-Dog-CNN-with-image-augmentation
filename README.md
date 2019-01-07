# Classification-of-Cat-and-Dog using CNNwith image augmentation
Classification of  images between two class cat and dog  using CNN
''
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
