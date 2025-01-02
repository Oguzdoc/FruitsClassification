# FruitsClassification

This project is a machine learning-based application for classifying fruits into five categories: Apple, Banana, Grape, Mango, and Strawberry. It includes scripts for training a model, evaluating its performance, and deploying it as a web application.

## Features

- **Training Script:** Build and train a MobileNetV2-based model for fruit classification using training and validation datasets.
- **Evaluation Script:** Evaluate the model's accuracy, generate confusion matrices, and save classification reports using test datasets.
- **Web Application:** Deploy the trained model via a Flask web app, allowing users to upload fruit images for real-time predictions.
- **Visualization:** Visualize dataset distribution and model performance metrics (accuracy, loss, confusion matrix).

## Folder Structure

```
FruitsClassification/
|-- Datasets/
|   |-- train/       # Training dataset
|   |-- valid/       # Validation dataset
|   |-- test/        # Test dataset
|
|-- Outputs/         # Outputs such as confusion matrix and metrics plots
|
|-- BuildTheModel.py # Training script
|-- ModelTesting.py  # Evaluation script
|-- App.py           # Flask application
|-- templates/
|   |-- index.html   # Web interface template
|-- static/
|   |-- styles.css   # CSS for styling the web app
|-- README.md        # Project documentation
```

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/FruitsClassification.git
   cd FruitsClassification
   ```

2. **Download or prepare datasets:**
   Organize your datasets into `train`, `valid`, and `test` folders under `Datasets/`, with subfolders for each fruit class.

3. **Train the model:**
   ```bash
   python BuildTheModel.py
   ```

4. **Evaluate the model:**
   ```bash
   python ModelTesting.py
   ```

5. **Run the web application:**
   ```bash
   python App.py
   ```

6. **Access the web application:**
   Open a web browser and navigate to `http://127.0.0.1:5000`.

## Requirements

- Python 3.7+
- TensorFlow
- NumPy
- Matplotlib
- Flask
- scikit-learn
- OpenCV

## Usage

1. Upload an image of a fruit through the web interface.
2. View the predicted fruit type and the model's confidence score.
3. Explore the classification results, confusion matrix, and training metrics in the `Outputs/` folder.

## License

This project is licensed under the MIT License. See `LICENSE` for more details.