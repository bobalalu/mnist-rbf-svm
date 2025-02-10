# Task: MNIST Dataset Classification using RBF-SVM

This repository contains a Jupyter Notebook that demonstrates how to use a Radial Basis Function (RBF) Support Vector Machine (SVM) for categorizing the MNIST dataset. The goal is to accurately classify the 28x28 grayscale images of handwritten digits (0–9) in the MNIST dataset without employing neural networks or deep learning techniques.

## Table of Contents

1. [Requirements](#requirements)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Notebook Overview](#notebook-overview)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

## Requirements

To run this notebook, you need the following Python packages installed:

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/bobalalu/mnist-rbf-svm.git
   cd mnist-rbf-svm
   ```

2. **Set up a virtual environment (optional but recommended):**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Start Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

2. **Open the Notebook:**
   Navigate to the `mnist_rbf_svm.ipynb` file and open it.

3. **Run the Notebook:**
   Execute the cells in the notebook sequentially to load the dataset, preprocess the data, train the RBF-SVM model, and evaluate its performance.

## Notebook Overview

The notebook is structured as follows:

1. **Loading the Dataset:**

   - The MNIST dataset is loaded using Scikit-learn's `fetch_openml` function.

2. **Data Preprocessing:**

   - The dataset is split into training and testing sets.
   - The pixel values are normalized to the range [0, 1].

3. **Model Training:**

   - An RBF-SVM model is initialized using Scikit-learn's `SVC` class with the `kernel='rbf'` parameter.
   - The model is trained on the training dataset.
   - The model is tested on the testing dataset.

4. **Model Evaluation:**

   - The trained model is used to make predictions on the test dataset.
   - The accuracy of the model is calculated and displayed.
   - A confusion matrix is plotted to visualize the classification results for the training and testing datasets.

5. **Hyperparameter Tuning (Optional):**

   - Grid search is performed to find the best hyperparameters (`C` and `gamma`) for the RBF-SVM model.

6. **Visualization:**
   - Some sample images from the test set are displayed along with their predicted labels.

## Results

After running the notebook, you should see the following outputs:

- **Accuracy:** The accuracy of the RBF-SVM model on the test set.
- **Confusion Matrix:** A visual representation of the model's performance across different classes.
- **Sample Predictions:** A few sample images from the test set along with their predicted labels.

## Contributing

Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please open an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to modify this README to better suit your project's needs. Happy coding!
