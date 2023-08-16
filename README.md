# FSM-INT-2023
The proposed development introduces an advanced defect detection system 
that leverages Machine Learning and Computer Vision to achieve rapid, 
accurate, and automated identification of piston defects. This innovative 
solution offers real-time processing, intuitive visualizations, and adaptive 
learning, revolutionizing traditional manufacturing quality control practices 
and ensuring consistent product excellence.
Explanatory Data Analysis(EDA):
Directory Structure
In the directory structure for the dataset, which includes images of different piston 
components categorized into "Defected1", "Defected2", and "Normal".
Piston_Dataset/
├── Defected1/
│ ├── kumda_component1.png
│ ├── kumda_component2.png
│ └── ...
├── Defected2/
│ ├── kumda_component1.png
│ ├── kumda_component2.png
│ └── ...
└── Normal/
 ├── kumda_component1.png
 ├── kumda_component2.png
 └── ...
About the dataset:
I created plots to visualize the number of elements in each dataset folder, providing an 
overview of the dataset. The dataset contains total 285 images. There are three groups of 
Folders present in the dataset. 
Defected 1 It consists of different images of piston which are broken/shaped out /fallen. 
Defected 2 It consists of different images of piston which are Oily/grease/rust stains. 
Normal It consists of different images of piston which are Perfectly Normal. 
About the images:
Analyzing the number of elements in each dataset folder helps me understand the 
distribution of images.
Piston defect detection project, images play a pivotal role as they are the primary data input 
for the convolutional neural network (CNN) model. These images represent various 
components of pistons, encompassing both normal and defective instances.
Each image, typically in PNG format, is composed of pixels that capture intricate details of 
the piston's surface. These images showcase diverse defect types, such as scratches, cracks, 
or anomalies, along with normal components. The CNN model analyzes these pixel values 
and patterns to discern crucial features that differentiate between normal and defective 
pistons.
Model Selection:
Convolutional Neural Networks (CNNs) are a popular and powerful choice for image-related 
tasks like image classification, including piston defect detection.
The model selection process for piston defect detection involved a thoughtful approach to 
ensure optimal accuracy and efficiency. After considering various convolutional neural 
network (CNN) architectures, a customized CNN model was developed. The model 
comprises multiple convolutional and pooling layers, effectively capturing intricate features 
in piston images.
Building the Model:
Creating a Layer for Resizing and Normalization
Before we feed our images to network, we should be resizing it to the desired size. 
Moreover, to improve model performance, we should normalize the image pixel value 
keeping them in range 0 and 1 by dividing by 256. This should happen while training as well 
as inference. Hence we can add that as a layer in our Sequential Model.
Model Architecture:
We use a CNN coupled with a Softmax activation in the output layer. Also added the initial 
layers for resizing, normalization and Data Augmentation.
Convolutional Neural Network (CNN) model for piston defect detection. It starts with 
preprocessing layers for resizing and rescaling the input images, followed by a series of 
convolutional and max pooling layers to extract features from the images. The model then 
flattens the output and passes it through fully connected dense layers, leading to the final 
output layer with softmax activation for classification into different defect classes.
Performance Evalution:
The model's performance is evaluated on the test dataset (test_ds), and the evaluation 
scores, including loss and accuracy, are stored in the scores variable. These metrics provide 
insights into how well the model generalizes to new, unseen data, helping to assess its
overall performance.The evaluation of the model on the test dataset yielded impressive results, with a low loss 
value of 0.0051 and a high accuracy of 100%, indicating that the model is performing 
exceptionally well on unseen data
