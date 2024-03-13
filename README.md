# PandasAI-Tutorials-PandasAI-with-Groq
#link to create groq API (https://wow.groq.com/)

from dotenv import load_dotenv

load_dotenv(override=True)


import pandas as pd
data = pd.read_excel('give your data path')
data.head()


import os

# Define the environment variable
os.environ["copy pest your api key"] = "your_api_key"


# Import the langchain_groq module
from langchain_groq.chat_models import ChatGroq


# Create a ChatGroq object
llm = ChatGroq(
    model_name="mixtral-8x7b-32768",
    api_key=os.environ["copy pest your api key"]


    # %%
from pandasai import SmartDataframe
df = SmartDataframe(data, config={"llm": llm})


# %%
# Define the environment variable
os.environ["your_api_key"] = "your_api_key"

# Import the langchain_groq module
from langchain_groq.chat_models import ChatGroq


# Create a ChatGroq object
llm = ChatGroq(
    model_name="mixtral-8x7b-32768",
    api_key=os.environ["your_api_key"]


    # %%
df.chat('total calls')


