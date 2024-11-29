# Integrate LLMs with Applications
<p align="center">
  <img src="https://img.shields.io/badge/python-%20-blue.svg?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Anaconda-%20-blue.svg?logo=anaconda&logoColor=white" alt="Anaconda">
</p>

This project demonstrates how to integrate Large Language Models (LLMs) into applications using IBM Cloud's Watson Machine Learning API. The project utilizes Python and Streamlit to create a simple application that communicates with the IBM Watson ML API to perform various language tasks like text generation, question answering, and data extraction.

## Requirements

Before starting, ensure you have the following installed:

- **Anaconda Environment**
- **Python**

### Required Libraries (from `requirements.txt`):

```text
load_dotenv==0.1.0
ibm_watson_machine_learning==1.0.345
ibm-cloud-sdk-core==3.16.7
streamlit==1.31.0
python-dotenv==1.0.0
  ```

## Installation
Install Anaconda and configure it as your Python interpreter in VSCode or another IDE.
Open your IDE and use Ctrl + Shift + P to select the Anaconda environment as the interpreter.

1. Clone the Repository:

```bash
git clone https://github.com/username/Integrate_LLMs_with_applications.git
 ```
2. Change to the Project Directory:

```bash
cd Integrate_LLMs_with_applications
```

3. Install Dependencies: Run the following commands to install the required libraries:

```bash
pip install -r requirements.txt
pip install ibm-watson-machine-learning
pip install ibm-cloud-sdk-core
pip install streamlit
```
4. Running the Application
To run the Python script and use the Watson Machine Learning API, execute:

```bash
python ./demo_wml_api.py
streamlit run demo_wml_api_with_streamlit.py
```

## Result
```bash
python demo_wml_api.py
---------------------------------------------------------------------------
Question/request: Write a paragraph about the capital of France.
Answer: Located in the east of France, Paris is the capital of France. It is also the most populated city of France with a population of 2.2 million people. It is the seat of the French parliament, the National Assembly. The city is located in the heart of France and is surrounded by the Île-de-France region.
---------------------------------------------------------------------------
C:\Users\LENOVO\anaconda3\Lib\site-packages\ibm_watson_machine_learning\foundation_models\utils\utils.py:273: LifecycleWarning: Model 'meta-llama/llama-2-13b-chat' is in deprecated state from 2024-08-26 until None. IDs of alternative models: None. Further details: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-lifecycle.html?context=wx&audience=wdp
warnings.warn(default_warning_template.format(
---------------------------------------------------------------------------
Prompt: 
 From the following customer complaint, extract 3 factors that caused the customer to be unhappy.
 Put each factor on a new line.

 Customer complaint:
         I just tried to book a flight on your incredibly slow website.  All
         the times and prices were confusing.  I liked being able to compare
         the amenities in economy with business class side by side.  But I
         never got to reserve a seat because I didn't understand the seat map.
         Next time, I'll use a travel agent!


 Numbered list of all the factors that caused the customer to be unhappy:


List of complaints: 1. Slow website
 2. Confusing times and prices
 3. Lack of understanding of the seat map
---------------------------------------------------------------------------
--------------------------Invocation with REST-------------------------------------------
Question/request: Write a paragraph about the capital of France.
Answer: Paris is the capital of France and the seat of government of the French Republic. The city is located in the heart of the Ile-de-France region, and its inhabitants are called Parisiens. The official name of the city is "Paris" (in French) or "Roubaix" (in Occitan).
---------------------------------------------------------------------------
```
