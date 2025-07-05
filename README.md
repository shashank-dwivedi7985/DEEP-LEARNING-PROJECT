This project demonstrates a convolutional neural network (CNN) for binary image classification — distinguishing between **cats** and **dogs** using TensorFlow and TensorFlow Datasets.
Developed and executed in **Google Colab**.


## 🚀 Project Overview

- **Goal:** Classify images as either cat or dog.
- **Dataset:** [`cats_vs_dogs`](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs) from TensorFlow Datasets.
- **Framework:** TensorFlow 2.x
- **Model:** Sequential CNN with 3 convolutional layers and dense output.



## 📁 Dataset Info

- **Total Images:** ~25,000
- **Corrupted Images Skipped:** ~1738
- **Image Shape:** Resized to 128x128 for faster training
- **Split:** 
  - 80% Training
  - 20% Validation



## 🛠️ Installation

```bash
!pip install tensorflow tensorflow-datasets matplotlib



📈 Training Result (1 Epoch)

Training Accuracy: 90.23%

Validation Accuracy: 81.49%

Training Loss: 0.2439

Validation Loss: 0.4800



📉 Accuracy and Loss Graphs


🖼️ Sample Predictions

Displays 9 images from the validation set with predicted labels.

for image, label in val_batches.take(1):
    predictions = model.predict(image)
    pred_labels = tf.round(predictions)

🧪 How to Run

1. Open this Colab Notebook.


2. Run all cells step by step.


3. View training, evaluation, and predictions.

📚 Future Improvements

Add dropout layers to reduce overfitting

Train for more epochs

Use transfer learning with pre-trained models like MobileNet or ResNet

Deploy model using Flask/FastAPI

📌 Acknowledgments

TensorFlow Team

TensorFlow Datasets

Google Colab

📄 License

This project is open-source and free to use under the MIT License.
