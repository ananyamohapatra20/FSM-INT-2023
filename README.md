# 🚀 FSM-INT-2023: Defect Detection in Mechanical Components

## 📌 Project Overview
**FSM-INT-2023** is a machine learning project aimed at identifying defects in mechanical components through image classification. Leveraging advanced techniques, this project trains models to differentiate between normal and defective components, contributing to improved quality assurance in manufacturing processes.

## 📊 Dataset
This project utilizes the **Mechanic Component Images** dataset, which can be accessed here:
- [Mechanic Component Images - Normal & Defected](https://www.kaggle.com/satishpaladi11/mechanic-component-images-normal-defected)

## 🗂 Repository Structure
```plaintext
FSM-INT-2023/
│
├── Deployment/
│   └── piston_defect_model.h5        # Trained model for deployment
│
├── Output/
│   └── flask_deployment.png           # Screenshot of the deployed Flask application
│
├── Reports/
│   └── Confusion_Matrix.png           # Visualization of model performance
│
├── SavedModel/
│   └── piston_defect_model.h5         # Saved model for inference
│
├── Piston_defect.ipynb                # Jupyter Notebook for training and evaluation
│
└── README.md                           # Project documentation
```

## ⚙️ Installation
To get started with this project, you will need the following:

### Prerequisites
- **Python 3.x**
- **Jupyter Notebook**
- Required libraries listed in `requirements.txt` (if available)

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/ananyamohapatra20/FSM-INT-2023.git
   cd FSM-INT-2023
   ```

2. Install the necessary packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook Piston_defect.ipynb
   ```

## 🛠 Usage
- **Load the dataset**: Follow the steps in the Jupyter Notebook to load and preprocess the images.
- **Train the model**: Use the provided code to train the model and evaluate its performance on the dataset.
- **Visualize results**: Review the generated confusion matrix and other relevant visualizations.
- **Deploy the model**: Explore the Flask application showcasing the trained model's capabilities.

## 🤝 Contributing
We welcome contributions! If you have suggestions or enhancements, please fork the repository and submit a pull request.

## 📝 License
This project is licensed under the MIT License. For more details, see the [LICENSE](LICENSE) file.

## 🌟 Acknowledgments
- A special thanks to the dataset authors for providing valuable resources that made this project possible.
- Thanks to the community for ongoing support and feedback.

## 📬 Contact
For questions or inquiries, feel free to reach out to me via GitHub.
