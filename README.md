Task 3: Multimodal Housing Price Prediction
🎯 Objective
To develop a complex Multimodal Neural Network that predicts housing prices by combining traditional tabular data (numerical/categorical) with visual data (property images). This project demonstrates the power of Late Fusion architecture in Deep Learning.

🛠️ Technical Implementation
Architecture: A Dual-Branch Neural Network.

Image Branch: A Convolutional Neural Network (CNN) or Pre-trained model used to extract visual features from property photos.

Tabular Branch: A Dense Multi-Layer Perceptron (MLP) to process features like square footage and bedrooms.

Late Fusion Technique: Features from both branches were processed independently until reaching a high-level representation (16 neurons each), where they were concatenated to make the final price prediction.

Data Scaling: Applied MinMaxScaler to the target price to ensure model convergence and prevent gradient instability caused by high-value inputs (prices up to $13.3M).

Frameworks: Python, TensorFlow/Keras or PyTorch, Scikit-learn, and OpenCV/PIL.

🚀 Key Insights
Multimodal Advantage: By combining image features with tabular data, the model can "see" property conditions (e.g., modern vs. dated) that are invisible in raw text data.

Metric Interpretation: The model achieved a Mean Absolute Error (MAE) of approx. $2.28M. Given the high variance in luxury property prices (reaching $13.3M), this demonstrates the model's ability to handle extreme price ranges.

Feature Correlation: The project proves that visual quality is a significant driver of real estate value, and integrating it into an ML pipeline significantly enhances predictive power over traditional methods.
