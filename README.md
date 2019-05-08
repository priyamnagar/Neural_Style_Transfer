# Neural Style Transfer
###
<strong>It applies neural style transfer in pytorch.</strong>

# Book_writer_LSTM
 ### 
<strong> It uses LSTM to learn writing a book character by character.</strong>

### Dateset
Download URL for the dataset is provided in the python notebook.

### Model description
* Here we are using pre-trained VGG19 model.
* To get the content and style representations of an image, we are passing an image forward through the VGG19 network until we get to the desired layer(s) and then get the output from that layer.
* To get style from the image we are using the Gram matrix. We extract features from our images and calculate the gram matrices for each layer in our style representation.
* Loss is calculated using the below function.

       torch.mean((target_features['conv4_2'] - content_features['conv4_2'])**2)
      
### How to Contribute
Find any typos? Have another resource you think should be included? Contributions are welcome!

* Fork this repository.

* Clone the repository to your desktop to make changes.

      $ git clone {YOUR_REPOSITORY_CLONE_URL}

* Issue a pull request by clicking on the green pull request icon.

Instead of cloning the repository to your desktop, you can also go to README.md in your fork on GitHub.com, hit the Edit button (the button with the pencil) to edit the file in your browser, then hit the Propose file change button, and finally make a pull request.

### License
This repository has been licensed under Apache 2.0.
