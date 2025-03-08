# DALLE-IMAGE-GENERATION
This project demonstrates how to generate an image using OpenAI's DALL-E model through Python.
## **Features**

- Generates an image based on a given text prompt.
- Uses DALL-E 3 model to produce high-quality images.
- Output includes a URL for the generated image.

## **Requirements**
Make sure you have the following installed:

- Python 3.7 or higher
- OpenAI Python library
## **Installation**
1. Install the OpenAI Python package:
```sh
pip install openai
```
## **Configuration**


1. Obtain your OpenAI API key from [OpenAI](https://openai.com).

2. Set up your API key in the script:
```sh
from openai import OpenAI
client = OpenAI()
```
## **Usage**
1. Run the script to generate an image:
```sh
from openai import OpenAI

client = OpenAI()

response = client.images.generate(
    model="dall-e-3",
    prompt="whale fish",
    size="1024x1024",
    quality="standard",
    n=1,
)

print(response.data[0].url)
```
