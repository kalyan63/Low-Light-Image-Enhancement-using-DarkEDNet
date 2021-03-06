# DarkEDNet

This is a CNN based model which includes encoder and decoder along with some connected CNN layers to enhance a low light images.
This is a supervised model which uses rmse as a loss function. We can use psnr or mae for loss as well. 
This model is mainly designed to retain most of the image features like colour and resolution. This model uses a lot less parameters than the previous SOTA models. 

1. **How to use our model:** 

    > The "Final Model.ipynb" Contains our model.
    
    > We have trained our model using LoL dataset. The formate of this folder is that it contains Test and Train folders. Both these folders contains high and low folder, which containes images with dark images and Bright images with same names. Test dataset has been provided, But you have to download Train dataset(LoL dataset) if you want to train the model on your own. 

        Test
        ----> high
        ----> low
        Train
        ----> high
        ----> low

    > FinalModel contains our Trained model. So you can load our model and use it for enhancing dark images of LoL dataset. 

    > You can train our model on your own but you require device with: 

        > 16 CPUs or higher 
        > 64 GB RAM or higher (Prefered 100GB in Google cloud)
     > **To Train the model with low ram (8-16 GB) , use tfrecords to store the image data set and then train the model.** 
   
2. **Model Architecture:**
    > !['Model'](model_.png)
3. **Examples:**
    > !['Image1'](image1.jpg)
    > !['Image2'](image2.jpg)
    > !['Image3'](image3.jpg)
    > !['Image4'](image4.jpg)
