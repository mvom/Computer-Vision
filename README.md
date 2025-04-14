# Computer-Vision

INFO8010: Project proposal
 Wilfried MvomoEto1
 1Wilfried.MvomoEto@student.uliege.be (s226625)
 I.
 SECTION 1: PROJECT DESCRIPTION
 Crop diseases pose a major threat to food security, yet
 their rapid identification remains challenging in many
 regions of the world due to a lack of necessary infras
tructure. The widespread penetration of smartphones
 globally, coupled with recent advancements in computer
 vision made possible by deep learning, has paved the
 way for smartphone-assisted diagnosis of crop diseases.
 The aim of this project is to build a deep neural network
 capable of analyzing images captured by smartphones to
 quickly and accurately identify crop diseases.
 II. SECTION 2: DATA
 We are analyzing 54,306 images of plant leaves,
 which are categorized into 38 class labels. Each
 class label corresponds to a crop-disease pair, and
 our goal is to predict this pair from the image
 of the plant leaf. These images are sourced from
 the dataset available at the following repository:
 https://github.com/digitalepidemiologylab/
 plantvillage_deeplearning_paper_dataset.
 To
 train our AI-based image recognition system, we will
 utilize this dataset.
 In all our experiments, we utilize three different ver
sions of the PlantVillage dataset. We begin with the
 original dataset in color, then we explore a grayscale
 version, and finally, we conduct our experiments on a
 version where the leaves are segmented. This approach
 allows us to assess the performance and robustness of
 our image recognition system in various contexts. We
 analyze how variations such as color, grayscale, and leaf
 segmentation can impact the model’s results. By under
standing how our system behaves under these different
 conditions, we can better evaluate its ability to general
ize and operate effectively in real-world environments.
 These three versions of the data are already available
 via the above-mentioned link.
 III. SECTION 3: COMPUTING RESOURCES
 If possible, we require access to powerful computers
 with GPU capabilities to train our deep convolutional
 neural network, as we have a large number of images to
 process.
 IV. SECTION 4: NEURAL NETWORK
 ARCHITECTURE
 For our convolutional neural network architecture, we
 draw inspiration from the pioneering AlexNet model
 proposed by Krizhevsky et al. in 2012 which has
 been applied for image-based plant desease detection[1].
 AlexNet comprises five convolutional layers followed by
 three fully connected layers. The architecture includes
 max-pooling layers and employs the ReLU activation
 function to introduce non-linearity. Dropout layers
 might be also incorporated to prevent overfitting. Batch
 normalization is another key component introduced in
 AlexNet to accelerate the training process.
 We plan to adapt and modify the AlexNet architec
ture to suit our specific task of crop disease identifica
tion. While the original AlexNet was designed for the
 ImageNet dataset, which consists of a thousand differ
ent classes, we will adjust the output layer to accommo
date our classification task, which involves predicting
 the crop-disease pair from input images of plant leaves.
 Our modified architecture will retain the fundamen
tal principles of AlexNet, including its convolutional and
 fully connected layers, activation functions, and regular
ization techniques. However, we will fine-tune the hy
perparameters and possibly introduce additional layers
 or modifications to optimize performance for our specific
 dataset and task.
 By leveraging the proven architecture of AlexNet and
 customizing it for our crop disease identification task, we
 aim to develop a deep neural network capable of accu
rately classifying plant leaf images and facilitating rapid
 diagnosis of crop diseases using smartphone technology.
 [1] Sharada P Mohanty, David P Hughes, and Marcel
 Salath´ e. Using deep learning for image-based plant dis
ease detection. Frontiers in plant science, 7:215232, 2016.
