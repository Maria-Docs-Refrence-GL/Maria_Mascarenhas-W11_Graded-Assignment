# 🩺 Breast Cancer Prediction Microservice 🩺
# Welcome to the Breast Cancer Prediction Microservice repository! 🎉

This project demonstrates how to create a microservice using the Python Flask framework to serve a machine learning model for predicting breast cancer diagnoses. With this microservice, you can easily deploy a powerful ML model to make real-time predictions. 🚀

# 🌟 Features
ML Model Training: Trains a machine learning model using the Breast Cancer Wisconsin (Diagnostic) dataset.
Flask Web Application: A Flask-based web application serving the ML model as a microservice.
Endpoints for Interaction:

GET /info: Get basic information about the microservice.
POST /predict: Submit data to get predictions about cancer type.

# 📦 Getting Started

1. Set Up Your Environment
Host an Ubuntu Virtual Machine using Oracle VM VirtualBox.
Set up Visual Studio Code on your Ubuntu VM. Setup Instructions\

2. Install Python 3.10
Run the following commands to download and install Python 3.10:

sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.10
python3 --version  # Verify installation

# 3. Create and Activate a Virtual Environment

python3 -m venv venv
source venv/bin/activate

# 4. Install Dependencies

pip install -r requirements.txt

# 5. Train the Model

Train and save the machine learning model:
python code_model_training/train.py

# 6. Run the Web Application

Start the Flask web server:
flask run -p 5000

# 7. Building Docker Image and Running it 

sudo docker build -t my-python-app .
sudo docker run -p 5000:5000 my-python-app

# 📄 Contributing
Feel free to open issues or submit pull requests. We welcome contributions from the community! 🌍

# 📧 Contact
For any queries, please reach out to karthikdeshpandeabd@gmail.com.

Happy coding! 🚀
