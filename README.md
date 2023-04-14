# wesite-python

# Import library
from flask import Flask

# Create an App
app = Flask(__name__)

# Home page
@app.route('/')
def home():
    return "Welcome to my website!"

# About page
@app.route('/about')
def about():
    return "This is an example website created by Flask"

# Run the App
if __name__ == '__main__':
    app.run()
