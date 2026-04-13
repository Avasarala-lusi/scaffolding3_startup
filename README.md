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

There are some example URLs on the page you can click to try it out:

- Pride and Prejudice: `https://www.gutenberg.org/files/1342/1342-0.txt`
- Frankenstein: `https://www.gutenberg.org/files/84/84-0.txt`
- Alice in Wonderland: `https://www.gutenberg.org/files/11/11-0.txt`
- Moby Dick: `https://www.gutenberg.org/files/2701/2701-0.txt`

