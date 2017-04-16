Lecture 2 Notes
---------------


### Meta

teaching approach:
Start at highest level, go down a level, then down a level, then down a level


###

use vgg.model.save_weights('results/ft1.h5')

-> Read Keras documentation

self.get_batches(path, shuffle=False, batch_size=batch_size, class_mmode=None)
self.model.predict_generator(test_batches, test_batches.nb_sample)


np.savetxt(csv_filename, matrix, ???)


### "probability"

The probabilities were not probabilities, they were extreme, either very near 0 or very near 1.


### 



CNNs
----


### Fine tuning?

ImageNet network learns a lot about how images/the world looks

### Filters?

Gabor filters

Each filter gets placed pixel by pixel over the image to identify diagonal lines / orange->blue shifts, etc


### Many layers



/def Architecture. The dimensions of the weight matrix layers


Initialize weights with Xavier initialization

]

/def Linear model. Model with only one layer
/def Dense model. Synonym for a linear model







bcolz is a small poorly known library for binary serialization and serializing of numpy arrays





/def onehot encoding. vector with only one 1 in it, every other value as 0.. eg [0,0,1,0,0,0,0]


### VGG16 layers
```
lambda_1 (Lambda)
zeropadding2d_1 (ZeroPadding2D)
convolution2d_1 (Convolution2D)
zeropadding2d_2 (ZeroPadding2D)
convolution2d_2 (Convolution2D)
maxpooling2d_1 (MaxPooling2D)
zeropadding2d_3 (ZeroPadding2D)
convolution2d_3 (Convolution2D)
zeropadding2d_4 (ZeroPadding2D)
convolution2d_4 (Convolution2D)
maxpooling2d_2 (MaxPooling2D)
zeropadding2d_5 (ZeroPadding2D)
convolution2d_5 (Convolution2D)
zeropadding2d_6 (ZeroPadding2D)
convolution2d_6 (Convolution2D)
zeropadding2d_7 (ZeroPadding2D)
convolution2d_7 (Convolution2D)
maxpooling2d_3 (MaxPooling2D)
zeropadding2d_8 (ZeroPadding2D)
convolution2d_8 (Convolution2D)
zeropadding2d_9 (ZeroPadding2D)
convolution2d_9 (Convolution2D)
zeropadding2d_10 (ZeroPadding2D)
convolution2d_10 (Convolution2D)
maxpooling2d_4 (MaxPooling2D)
zeropadding2d_11 (ZeroPadding2D)
convolution2d_11 (Convolution2D)
zeropadding2d_12 (ZeroPadding2D)
convolution2d_12 (Convolution2D)
zeropadding2d_13 (ZeroPadding2D)
convolution2d_13 (Convolution2D)
maxpooling2d_5 (MaxPooling2D)
flatten_1 (Flatten)
dense_2 (Dense)
dropout_1 (Dropout)
dense_3 (Dense)
dropout_2 (Dropout)
dense_4 (Dense)
```

