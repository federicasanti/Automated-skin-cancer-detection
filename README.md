# Automated-skin-cancer-detection
Developement of an end-to-end deep learning pipeline for skin lesion classification (benign vs malignant).
​

🚀 Main steps to develope an end-to-end deep learning pipeline for skin lesion classification (benign vs malignant).

📊 1. Dataset Collection
- Collected and organized labeled dermoscopic images of skin lesions: (benign vs. malignant) (https://www.kaggle.com/datasets/bhaveshmittal/melanoma-cancer-dataset)
- Ensured clean dataset structure and balanced dataset.

🖼️ 2. Image Preprocessing & Data Augmentation
- Image resizing to fixed input dimensions (64x64)
- Pixel normalization
- Augmentation techniques during training to reduce overfitting (random horizontal/vertical flips, random rotations, zoom transformations)

🤖 3. Model Development (TensorFlow / Keras)

Implemented and compared multiple CNN architectures:
- Custom Sequential CNN
- VGG16 (transfer learning)
- EfficientNetB0 (transfer learning)
Each model was trained for multiple epochs and evaluated using consistent validation splits

📈 4. Model Evaluation

Models were evaluated based on:
- Accuracy
- Loss
- Precision
- Recall for malignant cases (primary metric)

⚠️ We are working on a medical classification task, therefore high recall for malignant cases is critical to reduce false negatives.

🔬 5. Hyperparameter Optimization

Performed systematic tuning of:
- Learning rate
- Number of epochs

🏆 6. Best Model Selection

The best-performing model was:

🥇 EfficientNetB0 : 

- 96.79% Recall (Malignant cases)
- 95.75% Overall Precision
This model provided the best balance between recall and precision while maintaining strong generalization performance.

🚀 7. Deployment

The final model was deployed using Hugging Face Spaces with an interactive user interface:

🔗 https://huggingface.co/spaces/federicasanti/skin-cancer-detection

Users can upload a skin lesion image and receive a real-time prediction (⚠️ Warning: this model is for educational and research purposes only. It does not in any way replace a professional medical diagnosis). 

🛠️ Main Technologies Used

Python:

-Numpy

-Pandas

-TensorFlow

-Sckit-learn

Hugging Face

📧 Contact
email: federica.santi1997@gmail.com
