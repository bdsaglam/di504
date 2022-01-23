
## Focal loss paper
https://arxiv.org/abs/1708.02002

Lin et al. proposed a novel loss function that improves training accuracy in 
highly imbalanced problems such as object detection. Focal loss is a modulated 
cross entropy loss, where the modulating factor downweighs losses for easy 
negative examples such as background in object detection problems. This prevents 
easy negatives to dominate loss function and adversely influence the training.
The paper also proposes a one-stage object detection model architecture, named RetinaNet, 
that uses focal loss. It surpasses the accuracy of all two-stage object detection models 
without compromising inference speed and proves the effectiveness of focal loss.
We use focal loss in our models with the hyperparameters suggested by the paper.

pt = ? (2) 1 − p otherwise,
FL(pt) = −(1 − pt)γ log(pt).

## EfficientNet

Tan and Le analyzed model scaling in convolutional neural networks and shown 
that when network depth, width, and resolution are balanced, the model performance
improves. They proposed a new scaling method parameterized with a single coefficient and
demonstrated that when the method is applied to scale existing CNNs such MobileNet, it 
achieves higher accuracy.
To test the effectiveness of the method on a novel model architecture, first, 
they perform a neural architecture search for a convolutional block constrained 
by number of FLOPs and create full networks by scaling this block with the proposed scaling method.
The family of such networks with different scales is named EfficientNets.
Then, they compare the performance of EfficientNets with other well-performing
convolutional neural networks such as ResNet, ResNext, DenseNet, InceptionNet, and etc on
several image classification datasets such as CIFAR, ImageNet, Flowers.
They show that EfficientNets achieve highest accuracy and faster inference on 
all datasets among all models with less parameters.

## Bag of Tricks for Image Classification with Convolutional Neural Networks
https://arxiv.org/abs/1812.01187
The paper by He et. al is a comprehensive ablation study on convolutional neural networks.
It investigates the impact of training techniques such as learning rate warming, label smoothing, transfer learning, weighting loss; and hyperparameters such as batch size, learning rate on three tasks image classification, object detection, and semantic segmentation with three CNNs ResNet-50 [9], Inception-V3 [1], and MobileNet [11].