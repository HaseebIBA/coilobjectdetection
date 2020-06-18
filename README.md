# Object Detection using Coil dataset 
### Dependencies
.Jupyter notebook
.Keras
.Python 3.0
.Matplotlib
.os and shuttle
.Numpy
Install dependencies using conda or you can also directly download it in jupiter from search box.

#### Test Train Validation Split
The dattaset contains 360 images in order to classify 5 objects. all the data is mixedup together in the data set so firt you need to apply preprocessing in order to split data into train test  and validation.so 
.first you have to copy you dataset on in the in your C directory where your ipynp file used to get saved.
.second is to make directories of train test and validate by using os library. 
.Then each folder will have 5 subfolder because of it has 5 classes 
.then by using shuttle randomly pick each object image and paste them in train test and validate by dividing 80%,10% and 10% repectively.
now your dataset is ready...

### Model
then create model or fit model using keras which is going to use hidden layers by using relu actuivation function and in last softmax as we have more than 2 classes to identify.
then printing the summary of model to check the deescription of model.
after that use optimizer then use imageDatagenerator and fir the model with 5 epochs or your own choice 10 is enough with 5 validation number. and save the model

### Analysis
now using matplot lib anlysis the accuracy and loss and print it
this will show you whther your model is working perfectly or not. 

### Test
atlast pick any image froo the test dataset and resize it.
after resizing predict it from the model and also print it mean show the skected image using matplotlib.
