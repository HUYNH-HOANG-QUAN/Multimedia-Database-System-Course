# Boolean Retrieval Model

Educational implementation of a Boolean information retrieval system
over a speech corpus, with phrase matching and proximity search.


## Table of Contents

- [How It Works](#how-it-works)
- [Requirements](#requirements)
- [Running the Application](#running-the-application)
- [Example Queries](#example-queries)
- [Dataset](#dataset)
- [Notes](#notes)
- [Author](#author)
- [License](#license)


## How It Works

1. Documents are loaded from the speech corpus.
2. Text is cleaned by:
    - converting to lowercase
    - removing punctuation
    - handling contractions
    - removing stopwords
    - applying stemming
3. An inverted index is created for Boolean retrieval.
4. A positional index is created for phrase and proximity queries.
5. Queries are processed using Boolean logic and evaluated against the index.


## Requirements

- Python 3.x
- Flask
- NumPy
- Pandas
- NLTK

Install dependencies:

```bash
pip install flask numpy pandas nltk
```


## Running the Application

From the project root, run:

```bash
python main.py
```

Then open the app in a browser:

```
http://localhost:5000/
```


## Example Queries

The system supports queries such as:

```
united OR plane
biggest AND ( near OR box )
NOT (united AND plane)
actions AND wanted
"Hillary Clinton"
after years /1
develop solutions /1
```


## Dataset

The repository uses a set of 56 speech documents:

```
Trump Speechs/Trump Speechs/speech_0.txt
Trump Speechs/Trump Speechs/speech_1.txt
...
Trump Speechs/Trump Speechs/speech_55.txt
```


## Notes

This project is intended as an educational implementation of information
retrieval concepts. It is useful for learning:

- indexing
- Boolean logic
- phrase matching
- proximity searches
- text preprocessing


## Author

Original project by Muhammad Taha Khan.


## License

No explicit license file was found in the repository.
Please check the repository owner’s licensing terms before reusing or
redistributing the code.
