# Face-Recognition-using-Transfer-Learning 
#### A Machine Learning model for Facial Recognition by applying the Transfer Learning Technique on the VGG16 model over ImageNet data.

![](https://s3.ap-south-1.amazonaws.com/techleer/309.jpg)

#### "Transfer learning" makes use of the knowledge gained while solving one problem and applying it to a different but related problem.
###### For example, the knowledge gained while learning to recognize cars can be used to some extent to recognize trucks.

![](https://miro.medium.com/max/1400/0*sBn3nEeL3iGiCb_X.png)
#### Pre-Training
###### When we train the network on a large dataset(for example ImageNet), we train all the parameters of the neural network, and therefore the model is learned. It may take hours on your GPU.
###### Deep learning systems and models are layered architectures that learn different features at different layers (hierarchical representations of layered features). These layers are then finally connected to the last layer (usually a fully connected layer, in the case of supervised learning) to get the final output. This layered architecture allows us to utilize a pre-trained network (such as Inception V3 or VGG) without its final layer as a fixed feature extractor for other tasks.
![](https://miro.medium.com/max/1400/0*pqgIixh63w78lbQj.png)
#### The key idea here is to just leverage the pre-trained model’s weighted layers to extract features but not to update the weights of the model’s layers during training with new data for the new task.
#### Fine Tuning
###### We can give the new dataset to fine-tune the pre-trained CNN. Consider that the new dataset is almost similar to the original dataset used for pre-training. Since the new dataset is similar, the same weights can be used for extracting the features from the new dataset.
###### If the new dataset is very small, it’s better to train only the final layers of the network to avoid overfitting, keeping all other layers fixed. To remove the final layers of the pre-trained network. Add new layers. Retrain only the new layers.
###### If the new dataset is very much large, retrain the whole network with initial weights from the pre-trained model.

#### My story for complete guide of the project : 
##### visit --->  https://medium.com/@rajansh87/face-recognition-using-transfer-learning-2526c284a911 
