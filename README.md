A project on the implementation of Principal Components Analysis (PCA) for face recognition in Python. Initially, every image in the training set is transformed into vectors. PCA is a dimension reduction technique using eigenvalues and eigenvectors that have been decomposed from the covariance matrix of the training vectors. Hence, the eigenfaces are a set of eigenvectors that projects facial patterns on the space and is the basis for PCA face recognition method. Then, we get the weights of each eigenface so that we can achieve the capability to classify unknown faces using a distance algorithm. After that, once we got the testing result, we use it to do some analysis on our PCA to observe its performance over different parameters.

The entire process of our project can be summarized into training and testing phases. In the training and testing phase, we will use the images stored in the “Training_Images” and “Testing_Images” directories respectively. Each image is labeled in the format of “<identity>_<expression>” with a maximum of 5 images and 2 images for testing and testing respectively. In total, there will be 122 training images and 35 testing images.

This project also handles the ability to cope with in-plane rotation of the training and testing images, each of the images before resize will undergo a rotation_face() method which will rotate their faces based on the angle between the eyes and the Haar cascade is used to detect the eyes position within the data images. From there, the images will be rotated based on the center of the images. Furthermore, for this project, face images with face masks for training and testing are also included to improve the capability of our PCA face recognition model.
