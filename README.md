# GoogleLandmarkComputerVision

This repo contains an implementation of the Google landmark recognition, based off existing code from https://github.com/mayukh18/Google-Landmark-Recognition-Retrieval-2019.
This implementation uses a RESNET50 model trained on a subset of the training data to optimize for common cases, pretrained on imagenet. 
The last layer is chopped off of the trained model to extract feature vectors, which are used for a FAISS similarity search using the training set as the index to produce the final prodiction
Other advancements include using secondary models to filter for non-landmark images.
