## NetOCR: A Lightweight OCR Model

### 📖 Overview

NetOCR is a lightweight Convolutional Neural Network (CNN) designed for Optical Character Recognition (OCR).
Unlike heavy deep architectures like ResNet-18, NetOCR focuses on efficiency, fewer parameters, and competitive accuracy, making it suitable for real-world OCR tasks where speed and memory usage are critical.

| Model                     | Total Parameters | Trainable Parameters | Accuracy | Key Notes                                              |
| ------------------------- | ---------------- | -------------------- | -------- | ------------------------------------------------------ |
| **ResNet-18**             | 11,187,682       | 11,187,682           | \~96%    | Deep residual architecture, high complexity            |
| **NetOCR (Proposed CNN)** | **424,738**      | **424,738**          | \~95%    | Lightweight CNN, faster training, low memory footprint |

### 📊 Training Results

#### ResNet-18

Accuracy: High training accuracy (>98%) but validation accuracy saturates around 95–96%.

Loss: Training loss decreases steadily, validation loss fluctuates indicating mild overfitting.

Drawback: Requires large computational resources due to 11M+ parameters.
<img src="Output\restnet18.png"></img>

#### NetOCR (Proposed CNN)

Accuracy: Achieves >94% validation accuracy with stable training.

Loss: Both training and validation loss decrease consistently with less gap, showing good generalization.

Advantage: Only 424K parameters, ~26x fewer parameters than ResNet-18.

![App Screenshot]("C:\PROJECTS\OCR\Output\cnn.png")

### ✅ Why NetOCR is Better

#### Lightweight:

NetOCR has 424,738 parameters, compared to 11,187,682 in ResNet-18.

Requires far less memory, making it deployable on edge devices and mobile platforms.

#### Faster Training & Inference:

Trains significantly faster with fewer computations.

Ideal for real-time OCR applications.

#### Generalization:

Despite being smaller, NetOCR maintains competitive accuracy.

Training vs validation curves show less overfitting compared to ResNet-18.

#### Practical for Deployment:

Can be integrated in low-resource environments (IoT, embedded devices).

Efficient without sacrificing much accuracy.

#### OCR Outputs

### Restnet18:

![App Screenshot]("C:\PROJECTS\OCR\Output\restnet18_ocr.png")

#### NetOCR:

![App Screenshot]("C:\PROJECTS\OCR\Output\Proposed_cnn_ocr.png")

### 🚀 Conclusion

NetOCR demonstrates that lightweight CNNs can achieve near state-of-the-art performance in OCR tasks while being highly resource-efficient.
This makes it a strong alternative to deeper architectures like ResNet-18 when working with limited hardware or real-time deployment scenarios.
