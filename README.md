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

# 1. Set Up Your Environment
Host an Ubuntu Virtual Machine using Oracle VM VirtualBox.
Set up Visual Studio Code on your Ubuntu VM. Setup Instructions\

# 2. Install Python 3.10
Run the following commands to download and install Python 3.10:

sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.10
python3 --version  # Verify installation

# 3. Clone Github repository

git clone https://github.com/Vikas098766/Microservices.git

# 4. Create and Activate a Virtual Environment

python3 -m venv venv
source venv/bin/activate

# 5. Install Dependencies

pip install -r requirements.txt

# 6. Train the Model

Train and save the machine learning model:
python code_model_training/train.py

# 7. Run the Web Application

Start the Flask web server:
flask run -p 5000

# 8. Test the application and make predictions using example calls

curl -X GET http://localhost:5000/info
curl -X GET http://localhost:5000/health

Command : curl -d '[{"radius_mean": 17.99, "texture_mean": 10.38, "perimeter_mean":
122.8, "area_mean": 1001.0, "smoothness_mean": 0.1184, "compactness_mean": 0.2776,
"concavity_mean": 0.3001, "concave points_mean": 0.1471, "symmetry_mean": 0.2419,
"fractal_dimension_mean": 0.07871, "radius_se": 1.095, "texture_se": 0.9053,
"perimeter_se": 8.589, "area_se": 153.4, "smoothness_se": 0.006399, "compactness_se":
0.04904, "concavity_se": 0.05373, "concave points_se": 0.01587, "symmetry_se":
0.03003, "fractal_dimension_se": 0.006193, "radius_worst": 25.38, "texture_worst": 17.33,
"perimeter_worst": 184.6, "area_worst": 2019.0, "smoothness_worst": 0.1622,
"compactness_worst": 0.6656, "concavity_worst": 0.7119, "concave points_worst":
0.2654, "symmetry_worst": 0.4601, "fractal_dimension_worst": 0.1189}]' \ -H
"Content-Type: application/json" \ -X POST http://0.0.0.0:5000/predict



# 9. Building Docker Image and Running it 

docker build -t my-python-app .
docker run -p 5000:5000 my-python-app

# 📄 Contributing
Feel free to open issues or submit pull requests. We welcome contributions from the community! 🌍

# 📧 Contact
For any queries, please reach out to lolitamascarenhas@gmail.com

Happy coding! 🚀
