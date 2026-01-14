# U-Net Semantic Segmentation on CamVid

This project implements a **high-performance U-Net model**, a fully convolutional encoder–decoder architecture
widely used for **pixel-level semantic segmentation** in modern computer vision.

The model is trained on the **CamVid Urban Scene Understanding dataset** and learns to classify every pixel into  
**32 semantic classes**, including buildings, roads, vehicles, pedestrians, sky, and vegetation.

The encoder captures rich spatial context, while the decoder restores fine-grained details using **skip connections**,
resulting in crisp segmentation masks that preserve object boundaries with high accuracy.


## 🔍 Project Highlights

- ✅ Clean and modular **PyTorch** training pipeline  
- ✅ **U-Net encoder–decoder architecture** with skip connections  
- ✅ **Real-time data augmentation** for robust learning  
- ✅ Custom **Dataset & DataLoader** for RGB images and label masks  
- ✅ **Dice Loss + Cross-Entropy Loss** for balanced optimization  
- ✅ Visualization of **predictions, ground-truth masks, and training curves**  
- ✅ Easy reproducibility with `requirements.txt`  

This project is well-suited for:
- 🚗 Autonomous driving research  
- 🧠 Semantic segmentation–based computer vision projects  
- 📁 Deep learning portfolios and academic demonstrations  


## 🧠 Model Architecture

* **Encoder**

  * Series of convolution + downsampling blocks
  * Captures high-level semantic information

* **Decoder**

  * Upsampling layers with skip connections from the encoder
  * Restores spatial resolution and object boundaries


## 📊 Dataset: CamVid

CamVid is a real-world urban scene dataset containing video frames with **pixel-wise semantic annotations**.

**Key characteristics:**

* Urban driving scenes
* Multiple object categories
* Suitable for semantic segmentation benchmarks

> ⚠️ The dataset is **not included** in this repository.
> Please download it separately from the official source and arrange it as shown in the project structure.


## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/unet-camvid-segmentation.git
cd unet-camvid-segmentation
```

Install dependencies:

```bash
pip install -r requirements.txt
```


This script:

* Loads the trained model
* Generates segmentation predictions
* Visualizes results alongside ground-truth masks



## 📈 Loss Function

The training objective combines:

* **Cross-Entropy Loss**
  Handles multi-class classification effectively

* **Dice Loss**
  Improves class balance and overlap accuracy, especially for small objects

This combination leads to more stable and balanced segmentation performance.


## 🖼️ Visualization

The project supports visualization of:

* Input RGB images
* Ground-truth segmentation masks
* Model predictions
* Training and validation loss curves

These visual tools help in debugging and qualitative evaluation.



## 🔁 Reproducibility

* Fixed directory structure
* Clear configuration
* Dependency tracking via `requirements.txt`

With the same dataset and environment, experiments can be reliably reproduced.


## 📌 Applications

* Autonomous driving perception systems
* Smart city and traffic analysis
* Scene understanding research
* Portfolio projects for computer vision and deep learning


## 🙌 Acknowledgements

* U-Net architecture by Ronneberger et al.
* CamVid Dataset contributors
* PyTorch open-source community

## 👤 Author

**HOSEN ARAFAT**  

**Software Engineer, China**  

**GitHub:** https://github.com/arafathosense

**Researcher: Artificial Intelligence, Machine Learning, Deep Learning, Computer Vision, Image Processing**

