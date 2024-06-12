Project Statement - 
A Company wants to automate classificaiton of the objects enterign inot the port region and avoid human errors.
For this a database consisting of various typpes of sail objects are captured in a database

Dataset & Description -
Over 1200 images of boat classied into mainly 10 types have been captured in a dataset
Classes of boats are : Buoy, Cruise Ship , Ferry Boat , Froeght Boat , Gondola , Inflatable Boat , Kayak ,Paper Boat , Sail Boat

Task -
1. Build a CNN networ to classify the boat
2. Build a lightweight models with the aim of depoloying on a mobile device using transfer learning

Steps -
CNN MODEL :
1) Copy the dataset zip file in Google Drive & laod it on Colab notebook
2) Unzip the file in a new directory
3) Create Pandas Dataframe & split into Test train using train_test_split
4) Furthe split Train data into Train & Validation set
5) Using SMOTE balance the classes
6) Convert to Image Array usong Image Generator with flow_from_dataframeEc
7) Build a CNN model using Keras with layers as mentioned in the problem statement
8) Compile the model with ADAM optimiser , Categorical Cross entropy
9) TRain the model
10) Ealuate on tets data & print test loass * accuracy
11) Plot heatmap of the confusion matrix and print classification report

MOBILENETV2 MODEL :
1) Load MobileNetV2
2) Follow the layer building steps as given in the statement
3) Use Drouptout(0.1) & CallBAck

Compare the Accuracies & Test Loss of each model

