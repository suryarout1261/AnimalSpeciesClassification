🐾 Animal Species Detection using Deep Learning
This project aims to build an image classification system for animal species using deep learning techniques, particularly Convolutional Neural Networks (CNNs). The project explores and compares the performance of three prominent CNN architectures: ZFNet, VGG16, and GoogLeNet (Inception V1).

📖 Abstract
The goal is to detect and classify animal images into one of 10 species using deep learning. We implemented ZFNet, VGG16, and GoogLeNet, trained them from scratch on the Animals-10 dataset, and compared their performance based on accuracy, precision, recall, and inference time.

Best Model: GoogLeNet – 97% accuracy
Keywords: CNN, Image Classification, ZFNet, VGG16, GoogLeNet, Animal Detection, Deep Learning.

📂 Dataset
📌 Source: Animals-10 Dataset on Kaggle

📸 Images: ~28,000

🐕 Classes: 10

Butterfly, Cat, Chicken, Cow, Dog, Elephant, Horse, Sheep, Spider, Squirrel

🧠 Model Architectures
✅ ZFNet
5 convolutional layers + 3 fully connected layers

Smaller filters (7×7, 5×5, 3×3)

Performance: 45% accuracy

✅ VGG16
13 convolutional layers + 3 dense layers

Consistent use of 3×3 convolutions

Performance: 88% accuracy

✅ GoogLeNet (Inception V1)
Uses Inception modules for multi-scale feature extraction

Global average pooling instead of FC layers

Performance: 97% accuracy


📈 Results
Model	Accuracy	Best Class	Weakness
ZFNet	45%	Spider (900 correct)	Poor on Cat vs Dog
VGG16	88%	Dog (801 correct)	Overfit; Cat vs Dog confusion
GoogLeNet	97%	Spider (806 correct)	Some scattered mislabels

📌 GoogLeNet is recommended for deployment due to high accuracy and efficiency.

⚠️ Limitations
Limited to 10 animal classes.

Some confusion between visually similar animals.

No real-time deployment included.

Slight class imbalance and image variability affect generalization.

🔭 Future Work
Use ResNet, EfficientNet, or MobileNet for better accuracy/efficiency.

Integrate attention mechanisms or Grad-CAM for interpretability.

Address class imbalance via weighted losses or oversampling.

Explore deployment on mobile/embedded systems.
