# Abstract
Image segmentation finds applications in various fields, such as scene understanding, medical image analysis, video surveillance, augmented  reality and image compression. Over  the years, numerous  algorithms for image segmentation have been developed. However, with the  recent success of deep learning models in various vision tasks, there has been a significant focus on developing image segmentation approaches using deep   learning.

# Detailed Description
Image segmentation using deep learning is a computer vision task that aims to partition an image into meaningful regions. Deep learning models, particularly convolutional neural networks (CNNs), have proven highly effective for image segmentation. These models learn to automatically extract relevant features from the input image and classify each pixel into different categories or object classes.

The process begins by training the CNN on a labelled dataset, where each pixel is assigned a specific class or label. The network learns to identify patterns and textures associated with different objects or regions in the training images. During inference, the trained model takes an input image and predicts a segmentation mask, where each pixel is assigned a class label based on its visual characteristics.

Deep learning has shown remarkable success in image segmentation tasks by leveraging convolutional neural networks (CNNs) and advanced architectures like U-Net, Mask R-CNN, and Fully Convolutional Networks (FCNs). These models learn to extract high-level features and spatial.
Deep learning-based image segmentation has numerous applications, including medical imaging, autonomous driving, and object recognition. By accurately delineating object boundaries, this technique enables more precise analysis and understanding of images, leading to advancements in various fields. Additionally, researchers continue to explore and develop novel architectures and techniques to improve the performance and efficiency of deep learning-based image segmentation systems. (Minaee et al. 2020)

# Dataset
Clothing Co-Parsing (CCP) dataset is a new clothing dataset including elaborately annotated clothing items. The dataset comprises 1000 images and their respective semantic segmentation masks in PNG format. Each image and mask have dimensions of 825 pixels by 550 pixels. The masks are categorized various clothing items like shirts, hair, pants, skin, shoes, and glasses. (Yang et al. 2015)

# Architecture Proposal
ResUNet is an extension of the UNet architecture that incorporates residual connections from the ResNet model. It consists of a contracting path, an expanding path, and residual connections. The contracting path captures context information, while the expanding path aims for precise segmentation. Residual connections allow direct information flow between layers, mitigating the vanishing gradient problem and enabling more efficient learning. This combination of UNet's skip and ResNet's residual connections enhances the model's suggestive power, improving accuracy and robustness. ResUNet has demonstrated excellent performance in various image segmentation tasks, offering a powerful solution for tasks requiring precise localization and identification of objects in images.(Tomar 2021)![RESUNET_ARCH](https://github.com/SwarajSingh3005/ASE_Submission/assets/114939556/bb84ee68-d545-4130-9865-fa544a8cef9c)

Block diagram of the RESUNET architecture.(Tomar 2021)

![RESUNET_2-1024x648](https://github.com/SwarajSingh3005/ASE_Submission/assets/114939556/fca7c8a2-60a2-418c-a6a1-f1f5c3626439)

(a) Block diagram of the convolution block used in UNET and (b) residual block with identity mapping used in the proposed RESUNET.(Tomar 2021)



# Metrics and Evaluation
To assess the performance of deep learning-based image segmentation, these metrics are commonly used:

Intersection over Union (IoU) and Dice Coefficient: These metrics evaluate the overlap between the predicted segmentation mask (P) and the ground truth mask (G). They are calculated as:

IoU = (Area of Intersection) / (Area of Union)

Dice = (2 * Area of Intersection) / (Area of P + Area of G)

These metrics provide a measure of how well the predicted segmentation aligns with the ground truth, with values close to 1 indicating high accuracy. (Rezatofighi et al. 2019)



Mean Average Precision (mAP): Commonly used in object detection tasks, mAP evaluates the precision and recall of segmented objects. It considers various thresholds for defining positive or negative predictions and calculates the average precision across different object classes.

mAP = (Average Precision for Class 1 + Average Precision for Class 2 + ... + Average Precision for Class N) / N


This metric provides a comprehensive evaluation of segmentation performance across multiple object classes(Henderson and Ferrari 2016).

These evaluation metrics allow for quantitative assessment of the accuracy, boundary delineation, and overall quality of deep learning-based image segmentation. By comparing the performance of different models and techniques, researchers and practitioners can improve segmentation algorithms and achieve more accurate and reliable results.

# Reference
(Henderson and Ferrari 2016)
Henderson, P. and Ferrari, V., 2016. End-to-end training of object class detectors for mean average precision. arXiv [cs.CV] [online]. Available from: http://arxiv.org/abs/1607.03476 [Accessed 5 Jul 2023].
(Minaee et al. 2020)

Minaee, S., Boykov, Y., Porikli, F., Plaza, A., Kehtarnavaz, N. and Terzopoulos, D., 2020. Image segmentation using deep learning: A survey. arXiv [cs.CV] [online]. Available from: http://arxiv.org/abs/2001.05566 [Accessed 5 Jul 2023].
(Rezatofighi et al. 2019)

Rezatofighi, H., Tsoi, N., Gwak, J., Sadeghian, A., Reid, I. and Savarese, S., 2019. Generalized intersection over Union: A metric and A loss for bounding box regression. arXiv [cs.CV] [online]. Available from: http://arxiv.org/abs/1902.09630 [Accessed 5 Jul 2023].
(Sarda and Sun 2023)

Sarda, S. and Sun, T., 2023. Clothing segmentation for virtual try-on [online]. Stanford.edu. Available from: http://cs230.stanford.edu/projects_fall_2021/reports/103136976.pdf [Accessed 5 Jul 2023].

Tomar, N., 2021. RESUNET implementation in PyTorch [online]. Idiot Developer. Available from: https://idiotdeveloper.com/resunet-implementation-in-pytorch/ [Accessed 5 Jul 2023].

Yang, W., Luo, P. and Lin, L., 2015. Clothing co-parsing by joint image segmentation and labeling. arXiv [cs.CV] [online]. Available from: https://github.com/bearpaw/clothing-co-parsing#readme ,  http://arxiv.org/abs/1502.00739 [Accessed 5 Jul 2023].
