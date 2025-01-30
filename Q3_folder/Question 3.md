# How Pre-Training, Epochs, and Batches Affect Neural Network Performance

## Dataset:
Credit card clustering dataset: https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data
The dataset has been downloaded and added to the main branch of github.

## Research Question
For question 3 I have chosen to persue the 4th reseach question.

1. How does data augmentation affect the performance of a neural network?
2. How do parameters of a convolutional (or autoencoder) neural network affect
performance of a network?
3. How does choice of activation function affect the performance of a neural network?
4. How does pre-training (and epochs and batches) affect the performance of a neural
network? <---
5. How do choices about data such as i) amount of training data and ii) balance of
classes in a classification problem affect the performance of a neural network?

## Explanation

The question of how pre-training, epochs, and batch sizes affect the performance of a neural network is particularly relevant for this dataset, as it deals with unsupervised learning tasks such as clustering. Since the dataset does not have explicit class labels, using techniques like autoencoders or SOMs can help uncover meaningful patterns and clusters. 
Pre-training, along with tuning the number of epochs and batch sizes, plays a critical role in the performance of neural networks, especially for larger datasets.

Pre-training involves initializing the network’s weights through unsupervised learning methods before fine-tuning them for the clustering task. This can help the network learn useful features from the data and improve the quality of the resulting clusters. Tuning epochs (the number of iterations the network undergoes) and batch sizes (the number of samples 
processed before updating the weights) is also essential to achieving the optimal performance. Smaller batch sizes might lead to quicker convergence but can also result in noisy updates, while larger batch sizes provide more stable updates but might slow down the learning process.

To explore this, experiments can be designed to test the impact of pre-training, epochs, and batch sizes on customer segmentation. By comparing the performance with different configurations, insights can be gained regarding the best combination of these factors for improved customer segmentation. Evaluation metrics such as Silhouette Score, Cluster Purity, 
and Reconstruction Loss can help assess how well the model segments customers and how quickly it converges. This research will provide practical guidance for businesses on optimizing neural network training strategies for customer segmentation tasks.

In conclusion, the question about pre-training, epochs, and batch sizes is highly relevant and impactful for the customer segmentation problem at hand. It aligns well with the unsupervised nature of the task, and exploring these factors provides valuable insights that can improve segmentation accuracy and computational efficiency. This research question is 
the most directly applicable to real-world scenarios, offering actionable guidance for businesses seeking to optimize their customer segmentation models.
