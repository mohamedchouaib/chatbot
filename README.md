Disease Detection Chatbot
This repository contains two main components of a disease detection chatbot. The first component is a disease detection model, and the second is an NLP model responsible for processing user input to pass parameters effectively to the detection model.

Project Structure
model_of_detection.ipynb:

This notebook implements the disease detection model.
It takes input parameters (such as symptoms, duration, severity) to predict or detect potential diseases based on the data provided.
model_nlp.ipynb:

This notebook contains the NLP model that processes and interprets user inputs.
The processed output (parameters extracted from user input) is then formatted and passed to the disease detection model for evaluation.
Setup and Usage
Prerequisites
Python 3.x
Jupyter Notebook
Required libraries (install using pip install -r requirements.txt if a requirements file is included)
Running the Models
Prepare Environment:

Ensure all necessary libraries are installed. Run Jupyter Notebook in the directory containing the .ipynb files.
Running model_nlp.ipynb:

Open model_nlp.ipynb and run all cells to start the NLP model.
This will process input text (e.g., symptoms description) to extract parameters required by the detection model.
Running model_of_detection.ipynb:

Once model_nlp.ipynb has generated the necessary parameters, open model_of_detection.ipynb.
Input the parameters as indicated to make predictions about potential diseases.
Integrating the Chatbot Models
To use the chatbot in an interactive environment:

Integrate the NLP and detection models into a conversational framework (e.g., using Flask or FastAPI for an API, or a chatbot interface).
Process user input through the NLP model, then pass results to the detection model for a full pipeline from user input to disease prediction.
