# Chatbot Deployment with Flask and JavaScript

#PREVIEW
![Screenshot 2024-10-27 175445](https://github.com/user-attachments/assets/187b9df7-e336-4ea6-8673-5bb10fc95073)


This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.




![coffee-code](https://github.com/user-attachments/assets/8fadc4a1-34c9-407b-88bb-114b47caef75)



Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
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

Now for deployment to implement `app.py` and `app.js`.

