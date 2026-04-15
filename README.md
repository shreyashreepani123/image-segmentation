📌 Overview

This project implements pixel-wise image segmentation using Convolutional Neural Networks (CNN) and the powerful U-Net architecture.

The goal is to assign a class label to every pixel in an image, enabling fine-grained scene understanding — a key component in modern computer vision systems.

🧠 From autonomous driving to medical imaging — segmentation is everywhere.

🧠 Key Features

✨ High-quality semantic segmentation
✨ Implemented using U-Net architecture
✨ Modular training pipeline
✨ Efficient data generator for large datasets
✨ Clean separation of training & inference
✨ Supports real-world dataset (Cityscapes)

🗂️ Dataset

This project uses the Cityscapes Dataset, which focuses on urban scene understanding.

📊 Dataset Highlights:
🌍 Images captured across 50 cities
🚗 Real-world street scenes
🏷️ Originally 30 classes, reduced to:
Car 🚗
Road 🛣️
Person 🧍
Sky 🌌
Building 🏢
Tree 🌳
Background 🌫️
🏗️ Project Structure
image-segmentation/
│
├── train/
│   ├── model.py              # U-Net model architecture
│   ├── pre_processing.py     # Data preprocessing pipeline
│   ├── data_generator.py     # Keras data generator
│   ├── train.py              # Training script
│
├── test/
│   ├── post_processing.py    # Output mask generation
│   ├── test.py               # Inference script
│
└── README.md
⚙️ Installation
🔧 Prerequisites
Python 3.8+
pip / conda
GPU (recommended for training)
📥 Setup
# Clone repository
git clone https://github.com/shreyashreepani123/image-segmentation.git

# Navigate into project
cd image-segmentation

# Install dependencies
pip install -r requirements.txt
🏋️ Training the Model
python train/train.py
💡 What happens:
Loads dataset
Preprocesses images
Trains U-Net model
Saves trained weights
🔍 Inference / Testing
python test/test.py
🎯 Output:
Segmented image masks
Pixel-wise classified outputs
🧩 Model Architecture
🧠 U-Net Overview
Encoder (Downsampling path)
Bottleneck
Decoder (Upsampling path with skip connections)
Input Image
     ↓
[Conv → Pool] × N
     ↓
 Bottleneck
     ↓
[UpConv → Concatenate → Conv] × N
     ↓
 Segmentation Mask
📸 Results (Conceptual)
Input Image	Segmented Output
🏙️ Street Scene	🎨 Pixel-wise Mask
🚀 Applications

🔹 Autonomous Driving
🔹 Medical Image Segmentation
🔹 Satellite Image Analysis
🔹 Object Detection Preprocessing
🔹 Scene Understanding

🧪 Tech Stack
🐍 Python
🔥 TensorFlow / Keras
🧠 Deep Learning (CNN, U-Net)
📊 NumPy, OpenCV
📈 Future Improvements

🚧 Add more segmentation classes
🚧 Improve accuracy with DeepLabV3+ / Attention U-Net
🚧 Deploy as a web app (your next step 🔥)
🚧 Add real-time inference
🚧 Integrate with your MedPath AI project

🤝 Contributing

Contributions are welcome!

# Fork the repo
# Create your branch
git checkout -b feature/awesome-feature

# Commit changes
git commit -m "Added new feature"

# Push and create PR
📜 License

This project is licensed under the MIT License.

🙌 Acknowledgements
Cityscapes Dataset Team
Deep Learning Community
U-Net Paper Authors
⭐ Support

If you like this project:

🌟 Star the repo
🍴 Fork it
📢 Share it

👨‍💻 Author

Shreyashree Pani
📧 Connect • Build • Innovate
