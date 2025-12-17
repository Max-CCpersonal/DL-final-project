This project studies retinal disease classification from optical coherence tomography (OCT) images, a task that is essential for early ophthalmic diagnosis but traditionally relies on perfessional doctor interpretation. 
Using the publicly available OCT2017 dataset, we make the problem as a fourclass classification task involving choroidal neovascularization (CNV), diabetic macular edema (DME), DRUSEN, and normal retinal conditions. 
We adopt a transfer learning approach based on convolutional neural networks, evaluating three widely used architectures: ResNet-18 (He et al. 2016), EfficientNet-b0 (Tan and Le 2019), and MobileNetV2 (Sandler et al. 2018), 
all initialized with ImageNet pre-trained weights. 
Models are trained on the official training split dataset and evaluated on offical split test set of 968 images using accuracy, macro-F1, macro-precision, macro-recall, and confusion matrix analysis. 
All three models achieve consistently strong performance, with test accuracy ranging from 99.28-percent to 99.59-percent and macro-F1 scores exceeding 0.99, 
indicating balanced classification across all disease categories. Confusion matrices show that misclassifications are rare and primarily occur between clinically blurry related classes, such as DRUSEN and CNV. 
To enhance interpretability, Grad-CAM is applied to visualize class-discriminative regions, demonstrating that the models focus on anatomically meaningful retinal structures, 
even when the prediction is wrong. Overall, the results confirm the effectiveness of transfer learning and highlight the importance of explainable models in medical imaging applications.
