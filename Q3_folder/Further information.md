# Further Information about Question 3

## How Does Pre-Training (and Epochs and Batches) Affect Neural Network Performance?

Neural networks rely on proper training strategies to achieve high accuracy and generalization. Three key factors that influence performance are pre-training, number of epochs, and batch size. Each of these aspects plays a crucial role in how well the model learns and adapts to new data. 
This experiment explores their effects using a feedforward neural network trained on customer segmentation data.

## Pre-Training and Its Benefits

Pre-training is the process of initializing a neural network’s weights using a pre-trained model or an unsupervised learning phase before fine-tuning it with labeled data. One common pre-training approach is using an autoencoder, which learns to reconstruct input data before being used for classification tasks. 
Pre-training helps models converge faster and improves accuracy, as the network starts with meaningful feature representations instead of random weights. In our experiment, models with pre-trained weights performed better in terms of validation accuracy, confirming that pre-training helps generalization, particularly 
when data is limited or noisy.

## Impact of Epochs: Finding the Right Balance

The number of epochs determines how many times the model passes through the entire dataset during training. Too few epochs can result in underfitting, where the model fails to capture important patterns in the data. On the other hand, too many epochs may cause overfitting, where the model memorizes the training 
data but struggles with unseen examples. In our study, increasing the epochs from 50 to 100 showed some improvement, but after a certain point, the model's performance plateaued. This suggests that a higher number of epochs is only beneficial up to a threshold, beyond which early stopping should be applied to 
prevent overfitting.

## Effect of Batch Size on Training and Generalization

The batch size determines how many training samples are processed before updating the model’s weights. A smaller batch size (e.g., 32) provides more frequent updates, which can help the model generalize better but may also introduce instability due to higher variance in gradient updates. Conversely, a larger 
batch size (e.g., 64 or higher) smooths out updates, leading to faster training but potentially poorer generalization, as the model may get stuck in local minima. Our experiment confirmed this trend—models trained with batch size 32 showed slightly better validation accuracy than those trained with batch size 64, 
highlighting the benefits of smaller batches for generalization.
