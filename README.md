# General-Image-Classifier-App-F1-score-99.6-
General Image Classifier App F1 score=99.6%

General Image Classifier App F1 score=99.6%

This is a general purpose image classifier that can be applied to datasets that have the data organized as shown below. To use this code select Run all. The code will prompt the user to provide the required input data. It will take only a minute or so to enter the data and your model will be up and training. I have used this code on numerous data sets with excellent results. The model will initially run for 10 epochs. After 10 epochs you are prompted to enter H to halt training or you can enter an integer that specifies how many more epochs to run. After those epochs complete you will be again prompted to continue or halt training. The code shows the % decreasee  of the validation loss at the end of each epoch. This is a good guide to use to decide to continue or halt training. As you near the bottom of the loss function the % decrease in loss becomes smaller. I typically halt training when the % decrease falls below 5%. However sometimes it is best to continue training until the loss increases. The code then automatically lowers the learning rate. This often enables the model to again start decreasing the loss. Your saved model is always returned with the weights set to those for the epoch with the lowest loss.   

data directory  
* train directory    
  * class 0 
     * image 0 
     * image 1
     * ......
     * image m
  * class 1
     * image 0 
     * image 1
     * ......
     * image n 
  * ......
  * class m
     * image 0 
     * image 1
     * ......
     * image r 
* valid directory ( optional if there is no validation directory validation data is created by partition of train data)  
   * class 0 
     * image 0 
     * image 1
     * ......
     * image x
   * class 1
     * image 0 
     * image 1
     * ......
     * image y 
   * ......
   * class m
     * image 0 
     * image 1
     * ......
     * image z
* test directory ( optional if there is no test directory test data is created by partition of train data)  
   * class 0 
     * image 0 
     * image 1
     * ......
     * image a
   * class 1
     * image 0 
     * image 1
     * ......
     * image b 
   * ......
   * class m
     * image 0 
     * image 1
     * ......
     * image c
