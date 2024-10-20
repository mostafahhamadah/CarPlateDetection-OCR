Developed a system for car plate detection using TensorFlow and scikit-learn, with OCR handled by Tesseract. Labeled data via Label Studio and implemented in Jupyter Notebook. 
here is the link to the whole project including the dataset since uploading the dataset to github is limited to a certain size : 
https://drive.google.com/file/d/1HclMzJwEzx_DHgcV2l-hdqn-p5OAzdSp/view?usp=sharing 
hope u enjoy it  :)) 

Project Architecture
The system includes:

Data Labeling: Car images labeled using Label Studio.
Data Preprocessing: Annotations exported as XML and converted to CSV.
Model Training: A pre-trained InceptionV3 model for feature extraction with a custom head for bounding box regression.
Object Detection: Detects number plates in images.
OCR Integration: Text is extracted from number plates using Tesseract OCR.
Dataset Overview
Total Images: 228 images containing cars with visible number plates.
Variety: Images with different angles and lighting conditions to ensure robustness.
Training Details:
Optimizer: Adam (learning rate = 1e-6)
Loss: Mean Squared Error (MSE)
Batch size: 10
Epochs: 100
OCR Integration:
Tesseract OCR is used for text extraction from detected number plates.
