# Sign-Language-Recognition
This is an Indian Sign Language Recognition project using CNN (Convolutional Neural Networks) model. Using CNN, the model is trained to 
classify alphabets and digits. Speech Recognizer is used to spell the words and Hun-spell library acts 
as an autocorrect for the words produced. 
# Preprocessing
Each image in the dataset is converted from RGB to Grayscale format.The Canny Edge detector detects the edges of our hands therefore the shape of our hand acts as a parameter.Then the image is bit inverted i.e white color spaces and black color spaces are exchanged.

# Training
The image array is convolved with a 3X3 filter and then it is send to the Max pooling layer . This step is repeated twice.
The array is flattened. The dense layers are added to solve the complexities in our problem.
Four dense layers are used in our problem. Drop layer prevents our model from overfitting. Two drop layers are used.
1) ReLU (Rectified Linear Unit)
2) Softmax 
# Hyper Parameters used 
Train – 75% , Test – 25%.

Total training images -> 29673

Total test images -> 9906

Number of epochs = 14

Batch size = 10

Steps per epoch = 2625 (< No.of training images//Batch size)

Validation steps = 875.
