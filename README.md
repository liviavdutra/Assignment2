# Assignment2
Demo 1 – Cats and Horses
 

Part 1 – Transformers and Image Classification (7 points)
Here we want to compare how Transformers perform when compared to other kinds of networks for image classification, such as CNNs. Follow the tutorial hereLinks to an external site. in order to implement an image classification model.

The tutorial uses a model called ViT (Visual Transformer), which was the first transformer model to perform better at image classification than a CNN did.

As much as the tutorial would like you to login and upload your model to their hub, you do not need to do so for this assignment.

 

Part 2 – Using the COCO dataset (8 points)
The HuggingFace tutorial uses one of the datasets in its datasets package. We would like it to be able to be used with the data that we were using in our demo notebook.

Create/modify your own dataloader so that we can use the ViT model to differentiate the cats and horses found in the COCO dataset (i.e. the one from the demo notebook).

 

Part 3 – Multiclass Classification (8 points)
The original task was only with binary classification. Get it to do multiclass classification, preferably on similar kinds of targets (like the cats and horses example, as opposed to cats and airplanes). You can find a list of categories for the dataset hereLinks to an external site..

Do this both for the original CNN model and for the ViT model.

 

Part 4 – How does the classification work now? (7 points)
Do a comparison of the models, both quantitative and qualitative. How does the models’ performances vary from each other? Is one of the models better at specific things than the other? Or is one of them much better than the other? Moreover, are these differences the same between both the binary classification task and in a multiclass classification task?

 

Demo 2 – Chinese Word Segmentation
 

Part 1 – Transformers for Sequence Classification (7 points)
Here we want to compare how Transformers work when compared to other kinds of sequence to sequence networks, such as LSTMs. Follow the tutorial hereLinks to an external site. in order to implement a token classification model.

The tutorial uses DistilBERT, a smaller version of BERT designed to be used when we have less memory available. BERT itself is one of the most popular Transformer models both for sequence and for token classification.

 

Part 2 – Using BERT with Our Data (16 points)
The huggingface tutorial uses both an English dataset and a model pretrained in English. Change the code so that it can use the CONLL-U dataset from the demo notebook.

One of the major issues that you might find is that just changing the dataset will not yield the results we would expect. Because of that, you might also have to change the model you’re using. I wasn’t able to find a reasonably documented version of DistilBERT for Chinese, but HuggingFace has a Chinese BERTLinks to an external site. available.

Another thing to keep in mind is that BERT already segments the words as it things they should be segmented, so you will probably have to find a workaround in order to avoid the task being trivial (and to get a single label from each of your characters).

 

Part 3 – Performance Analysis (7 points)
Do a comparison between both models and how differently they perform. We are assuming that most of you don’t read Chinese, so we are not expecting much in the area of qualitative analysis.
