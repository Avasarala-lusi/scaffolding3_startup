# Text Preprocessing Web Service

A Flask web app that fetch books from Project Gutenberg, cleans up the text, and shows some basic stats about it.

## Setup

You'll need Python 3.9+.

1. Clone the repo and install dependencies:

```bash
pip install -r requirements.txt
```

2. Make sure everything is working:

```bash
python test_setup.py
```

You should see all checks passing (Python version, packages, Gutenberg access, etc).

3. Start the server:

```bash
python app.py
```

Then go to http://localhost:5000 in your browser.

## How to use it

Paste a Project Gutenberg `.txt` URL into the input box and hit submit. The app will download the book, strip out the Gutenberg headers/footers, normalize the text, and give you back:

- Word, sentence, and character counts
- Average word and sentence lengths
- The 10 most common words
- A short summary (first 3 sentences)
- A preview of the cleaned 500 characters

## Screenshot of working appliation
<img width="1816" height="847" alt="image" src="https://github.com/user-attachments/assets/d03721cb-f343-467b-b147-ec346a5730f1" />

<img width="1790" height="810" alt="image" src="https://github.com/user-attachments/assets/dbceba80-ddc5-43be-a27d-8ec3f6ef9942" />



