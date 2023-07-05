# Chatbot Deployment with Flask and JavaScript

<img width="500px" height="500px" src="https://im3.ezgif.com/tmp/ezgif-3-edb48303de.gif"/>
 ### **Chatbot Assistance**

**Purpose**: To provide round-the-clock customer service that can efficiently handle common queries and issues, improving customer satisfaction and freeing up staff for more complex tasks.

**Requirements**:

- An AI-based text chatbot integrated into the web application.
- Pre-programmed responses for common customer queries like "What is your operation hours?", "What is the status of my order?", etc.
- User-friendly interface for customers to interact with the chatbot.

**Metrics for success**: Decrease in basic customer inquiries handled by human staff and positive user feedback about the chatbot.

- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
Clone repo and create a virtual environment
```
$ git clone  
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```

Now for deployment follow my tutorial to implement `app.py` and `app.js`.
 

 
