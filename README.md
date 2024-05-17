# Image-Captioning

Dataset: 

consists of 8,000 images that are each paired with five different captions which provide clear descriptions of the salient entities and events. … The images were chosen from six different Flickr groups, and tend not to contain any well-known people or locations, but were manually selected to depict a variety of scenes and situations.

What is Image Captioning ?

Image Captioning is the process of generating textual description of an image. It uses both Natural Language Processing and Computer Vision to generate the captions.
This task lies at the intersection of computer vision and natural language processing. Most image captioning systems use an encoder-decoder framework, where an input image is encoded into an intermediate representation of the information in the image, and then decoded into a descriptive text sequence.

Image Feature Extraction ?
DenseNet 201 Architecture is used to extract the features from the images
Any other pretrained architecture can also be used for extracting features from these images
Since the Global Average Pooling layer is selected as the final layer of the DenseNet201 model for our feature extraction, our image embeddings will be a vector of size 1920

Modelling ?
The image embedding representations are concatenated with the first word of sentence ie. starseq and passed to the LSTM network
The LSTM network starts generating words after each input thus forming a sentence at the end


