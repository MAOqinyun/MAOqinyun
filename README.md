- 👋 Hi, I’m @MAOqinyun
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
MAOqinyun/MAOqinyun is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import openai
from flask import Flask, request, jsonify

app = Flask(__name__)

openai.api_key = "YOUR_API_KEY"

@app.route('/chat', methods=['POST'])
def chat():
    data = request.get_json()
    prompt = data['prompt']
    response = openai.Completion.create(
        engine="davinci",
        prompt=prompt,
        max_tokens=1024,
        n=1,
        stop=None,
        temperature=0.5,
    )
    message = response.choices[0].text.strip()
    return jsonify({'message': message})
    while(True):
    question = input("真人:")
    print("假机器人:" + question.strip("吗??") + "!")
    python
import tensorflow as tf
import numpy as np

# Define your model here

while True:
    question = input("真人:")
    # Use your model to generate a response
    print("假机器人:" + response + "!")
    
